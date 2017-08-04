# lots-o-ansible
Reference repo with lots of submodules of ansible roles, modules, playbooks, and tools.

Why? So they can be checked out, and searched with local tools
(ie, find, grep, ack, ag, etc) when looking for examples.


# Organization
There isn't much.

Roughly, repos that are at playbook level go into playbooks/.
Repos that are at role level go in roles/
Repos that are primarily modules go in modules/
Repos that are primarily tools go into tools/
Repos that are primarily docs go into docs.

Since repos of ansible setups typically include one or more
of the above, the organization is pretty arbitrary and subject
to change.


# Getting everything

You will want to clone recursively to get everything in one shot.

``` shell

git clone --recurse-submodules git@github.com:alikins/lots-o-ansible.git
```

For git 2.8+, the `--jobs` option may be useful to parallelize
some of the cloning.

It can be pretty large (1.7gb which last checked). Most of
the size comes from some of the submodules include pkgs and
other large files in their repos.


# Todo
- add a tool to transform the repo into an ansible playbook
- add tools for running various indexing tools (codesearch, ctags, global, etc)
- add tools for using the previously mentioned indexes (csearch, readtags, etc)


# License
This is primarily just a container for git submodules that point to various
repos of playbooks, roles, etc. So check the license provided by each submodule.
