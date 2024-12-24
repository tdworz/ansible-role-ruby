# Tom's Ruby Ansible Role

An Ansible role to install and configure Ruby.

## Available Variables

| Variable            | Type     | Default  | Description |
|:--------------------|:--------:|:--------:|:------------|
| ruby_install_method | string   | `repos`  | One of the following: `repos`. |
| ruby_version        | string   | `stable` | A semantic version number or keyword. If using a semantic version number, you must use one of the the following: just the major version (ie. `3`), the major-minor version (ie. `3.4`), or the major-minor-patch version (ie. `3.4.2`). Allowed keywords are: `latest`, `base`, or `stable`. |

#### Installing from Repos

##### RHEL and RHEL Derivatives

If you want to install Ruby from an application stream module, set
`ruby_version` to the stream (ie. `3.3`). The following table shows the
available streams known when this _README_ was last updated.

| Enterprise Linux Version | Stream | Ruby Version |
|:------------------------:|:------:|:------------:|
| 9                        | `base` | 3.0.x        |
| 9                        | `3.1`  | 3.1.x        |
| 9                        | `3.3`  | 3.3.x        |

By default, `ruby_version` is set to `stable` which corresponds to the `base`
stream. You may also set `ruby_version` to `latest` to use the latest stream.

## Copyright &amp; License

Copyright © 2024 Tom "tdworz" Dworzanski.

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program. If not, see <https://www.gnu.org/licenses/>.
