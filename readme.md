# Microfrontends (MFEs) using WebPack 5 Module Federation
# Install
(0. ``npm install --global yarn`` -- In case you don't have **yarn** installed)
1. ``yarn`` -- Install core dependencies (only **lerna** by default)
2. ``yarn bootstrap`` -- Install dependencies of all micro frontends and shell with lerna
3. ``yarn start`` -- Starts the shell and all Micro Frontends with lerna
4. ``http://localhost:4200`` -- default shell page URL

# Folders
*Also check out readme files inside each folder*
## ./shell 
``Angular 11.0.0-rc.2`` \
Core application, hosting microfrontends.

## ./mfe1
``Angular 11.0.0-rc.2`` \
Microfrontend #1 - Same Angular version as shell.\
Test basic MFE concept (an application rendered inside another one).

## ./mfe2
``Angular 11.0.0-rc.0`` \
Microfrontend #2 - Older Angular version. \
Test how MFEs of same framework but different versions works together (MFE #1 + MFE #2).


## ./mfe3
``Angular 11.0.0-rc.0`` \
Microfrontend #3 - Same Angular version as MFE #2. \
Test source files caching during routing between MFEs of same libs.


## ./mfe4 - react
``React 17.0.1`` \
Microfrontend #4 - React \
Test compatibility of MFEs built on different libs inside one shell.
