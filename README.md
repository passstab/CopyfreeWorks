# Copyfree Works

Copyfree works -- quite well, in fact.  As evidence, we maintain a [list of
copyfree works][list] on the Copyfree Initiative website.  This very small
project repository exists for the sole purpose of collaborative maintenance of
the datafile that lies behind that list.

## Contributing

If you have a project in mind to add to the works list, follow our process.

If you do not have a project in mind, have some time on your hands, and just
want to help out, check this project's issue tracker for tasks you could
undertake.  Some of them may be long tasks, involving lists of applications; if
you do not get through the complete list, just update the issue with a comment
about what you accomplished to make it easy on the next person to work on that
issue.  With that in mind, follow our process.

If you just want some project(s) added to the works list without doing any
appreciable work, add an issue.  We will get to it whenever we feel like it,
probably shortly after some higher-priority work.

Process:

1. Fork this repository.
2. Commit changes in your fork.  Use imperative language commit messages.
3. Use GitHub's facilities for a Pull Request.
4. Monitor the PR for any comments we may have on your PR.
5. Celebrate when your PR gets merged.  If it does not get merged for some
   reason, congratulate yourself on the learning experience.

(You get bonus points for using a descriptively named topic branch in your PR.)

Please use examples in the YAML datafile as your template for adding new
copyfree works.  At a bare minimum, a new suggestion should include project
name, license name, and URIs for both an authoritative license terms reference
and whatver passes for the project's "main" webpage (the `uri` value).  The
license terms reference should be authoritative *for the project*, and not
simply the address for some license text at OSI.

This is an example of the general format of works list datafile entries:

    Project Name:
      uri:
      - http://projectname.example/
      description:
      - Project Name does something useful.
      license:
      - MIT/X11 License
      license_reference:
      - http://github.com/project-name/ProjectNameMain/blob/master/LICENSE
      tags:
      - client
      - network
      - software

Any comments asking for changes -- no matter how trivial they may seem -- are
not intended to carry any negative emotional baggage, unless you are trolling
us.  They are intended to help you get used to how we do things, and to help us
find time to handle all the backlog of work building up as we plan for a
substantial reimplementation of the CI website, from infrastructure on up.  See
more on that later in this README.

Feel free to submit improvements to works already included in the list.
Especially among some of the earliest-added works, there is some missing
information in some entries, for instance, and sometimes linkrot causes
problems for some works in the list.

## Cautionary Notes

* Adhere to our YAML formatting style.  Otherwise, we will ask you to correct
  it, and/or end up spending extra time reformatting it ourselves.

* Have patience.  Sometimes it takes a little while for us to fill in the
  blanks in any incomplete submissions (e.g. anything that includes only the
  website and license reference addresses), or sometimes to investigate the
  project sufficiently well to verify that all the submitted information
  conforms to internal CI standards.

* This project may or may not be preserved for posterity when it becomes
  obsolete.  See more on that later in this README.

## Problems/Requests

Feel free to use the issue tracker for this project if you have concerns or
requests related to the works list in its current form, the future design of
the new works database, or the process we use for updating the current works
list.  Please use succinct, but complete, sentences in your ticket titles.

## Roadmap

This is where "later in this README" happens:

We intend to dramatically update the [Copyfree Initiative website][ci] in the
near-ish future.  One of the big changes will be the replacement of the current
works list system -- a simplistic YAML-backed webpage -- with a searchable,
sortable, filterable interface, backed by a PostgeSQL database.

* Yes, we do intend to ensure it is still accessible for people who block
  JavaScript, though it is possible (not yet decided) that some (non-critical)
  features will be added only when your browser allows JavaScript.

* Yes, we do intend to make the data we use for the new works DB available
  under a copyfree license, possibly even as YAML and/or JSON, though we have
  not yet really thought much about how we'll do that.  (We intend to provide
  the entire (new) codebase under a copyfree license, as well.)

[ci]: http://copyfree.org
[list]: http://copyfree.org/resources/works
