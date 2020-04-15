<p align="center">
  <a href="https://github.com/gr2m/twitter-together/issues/16"><img src="assets/logo.png" width="150" alt="twitter together logo" /></a>
</p>

<h1 align="center">Twitter, together!</h1>

For Open Source or event maintainers that share a project twitter account, `twitter-together` is a GitHub Action that utilizes text files to publish tweets from a GitHub repository. Rather than tweeting directly, GitHub’s pull request review process encourages more collaboration, Twitter activity and editorial contributions by enabling everyone to submit tweet drafts to a project.

## Why
We wanted to open up the LeicesterJS twitter account so community members could interact more closely with each other and be more collaborative as a meetup.
Rather than sharing username/passwords enmasse, we instead can all tweet from this central place (even with polls).

## How do I tweet?

To create a new tweet create a new `*.tweet` file in this `tweets/` folder.

<kbd>[Create new tweet](../../../new/master/?filename=tweets/<your-path>.tweet)</kbd>

### Example

Create a new file `tweets/hello-world.tweet` with the content

> Hello, world!

You can use subfolders, e.g. `tweets/2019-02/hello-world.tweet`, as long as the file is in the `tweets/` folder and has the `.tweet` file extension

### Create a tweet with a twitter poll

**Note**: The configured twitter account needs to be authorized to use Twitters Ads API in order to send tweets including a poll.

A tweet including a poll must end with 2-4 options in the following format

> Here is some text
>
> ( ) option A
> ( ) option B
> ( ) option C
> ( ) option D

### Notes

- Only newly created files are handled, deletions, updates or renames are ignored.
- `*.tweet` files will not be created for tweets you send out directly from twitter.com
- If you need to rename an existing tweet file, please do so locally using [`git mv old_filename new_filename`](https://help.github.com/en/articles/renaming-a-file-using-the-command-line), otherwise it may occur as deleted and added which would trigger a new tweet.

### Questions?

If you have any further questions or suggestions, please create an issue at https://github.com/leicester/twitter-together/issues/new
