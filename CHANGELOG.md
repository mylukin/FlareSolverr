# Changelog

## v3.3.25 (2025/06/14)
* Remove `use-gl` argument. Thanks @qwerty12
* u_c: remove apparent c&p typo. Thanks @ok3721
* Bump requirements

## v3.3.24 (2025/06/04)
* Remove hidden character

## v3.3.23 (2025/06/04)
* Update base image to bookworm. Thanks @rwjack

## v3.3.22 (2025/06/03)
* Disable search engine choice screen
* Fix headless=false stalling. Thanks @MAKMED1337
* Change from click to keys. Thanks @sh4dowb
* Don't open devtools
* Bump Chromium to v137 for build
* Bump requirements

## v3.3.21 (2024/06/26)
* Add challenge selector to catch reloading page on non-English systems
* Escape values for generated form used in request.post. Thanks @mynameisbogdan

## v3.3.20 (2024/06/21)
* maxTimeout should always be int
* Check not running in Docker before logging version_main error
* Update Cloudflare challenge and checkbox selectors. Thanks @tenettow & @21hsmw

## v3.3.19 (2024/05/23)
* Fix occasional headless issue on Linux when set to "false". Thanks @21hsmw

## v3.3.18 (2024/05/20)

* Fix LANG ENV for Linux
* Fix Chrome v124+ not closing on Windows. Thanks @RileyXX

## v3.3.17 (2024/04/09)

* Fix file descriptor leak in service on quit(). Thanks @zkulis

## v3.3.16 (2024/02/28)

* Fix of the subprocess.STARTUPINFO() call. Thanks @ceconelo
* Add FreeBSD support. Thanks @Asthowen
* Use headless configuration properly. Thanks @hashworks

## v3.3.15 (2024/02/20)

* Fix looping challenges

## v3.3.14-hotfix2 (2024/02/17)

* Hotfix 2 - bad Chromium build, instances failed to terminate

## v3.3.14-hotfix (2024/02/17)

* Hotfix for Linux build - some Chrome files no longer exist

## v3.3.14 (2024/02/17)

* Update Chrome downloads. Thanks @opemvbs

## v3.3.13 (2024/01/07)

* Fix too many open files error

## v3.3.12 (2023/12/15)

* Fix looping challenges and invalid cookies

## v3.3.11 (2023/12/11)

* Update UC 3.5.4 & Selenium 4.15.2. Thanks @txtsd

## v3.3.10 (2023/11/14)

* Add LANG ENV - resolves issues with YGGtorrent

## v3.3.9 (2023/11/13)

* Fix for Docker build, capture TypeError

## v3.3.8 (2023/11/13)

* Fix headless=true for Chrome 117+. Thanks @NabiKAZ
* Support running Chrome 119 from source. Thanks @koleg and @Chris7X
* Fix "OSError: [WinError 6] The handle is invalid" on exit. Thanks @enesgorkemgenc

## v3.3.7 (2023/11/05)

* Bump to rebuild. Thanks @JoachimDorchies

## v3.3.6 (2023/09/15)

* Update checkbox selector, again

## v3.3.5 (2023/09/13)

* Change checkbox selector, support languages other than English

## v3.3.4 (2023/09/02)

* Update checkbox selector

## v3.3.3 (2023/08/31)

* Update undetected_chromedriver to v3.5.3

## v3.3.2 (2023/08/03)

* Fix URL domain in Prometheus exporter

## v3.3.1 (2023/08/03)

* Fix for Cloudflare verify checkbox
* Fix HEADLESS=false in Windows binary
* Fix Prometheus exporter for management and health endpoints
* Remove misleading stack trace when the verify checkbox is not found
* Revert "Update base Docker image to Debian Bookworm" #849
* Revert "Install Chromium 115 from Debian testing" #849

## v3.3.0 (2023/08/02)

* Fix for new Cloudflare detection. Thanks @cedric-bour for #845
* Add support for proxy authentication username/password. Thanks @jacobprice808	for #807
* Implement Prometheus metrics
* Fix Chromium Driver for Chrome / Chromium version > 114
* Use Chromium 115 in binary packages (Windows and Linux)
* Install Chromium 115 from Debian testing (Docker)
* Update base Docker image to Debian Bookworm
* Update Selenium 4.11.2
* Update pyinstaller 5.13.0
* Add more traces in build_package.py

## v3.2.2 (2023/07/16)

* Workaround for updated 'verify you are human' check

## v3.2.1 (2023/06/10)

* Kill dead Chrome processes in Windows
* Fix Chrome GL erros in ASUSTOR NAS

## v3.2.0 (2023/05/23)

* Support "proxy" param in requests and sessions
* Support "cookies" param in requests
* Fix Chromium exec permissions in Linux package
* Update Python dependencies

## v3.1.2 (2023/04/02)

* Fix headless mode in macOS
* Remove redundant artifact from Windows binary package
* Bump Selenium dependency

## v3.1.1 (2023/03/25)

* Distribute binary executables in compressed package
* Add icon for binary executable
* Include information about supported architectures in the readme
* Check Python version on start

## v3.1.0 (2023/03/20)

* Build binaries for Linux x64 and Windows x64
* Sessions with auto-creation on fetch request and TTL
* Fix error trace: Crash Reports/pending No such file or directory
* Fix Waitress server error with asyncore_use_poll=true
* Attempt to fix Docker ARM32 build
* Print platform information on start up
* Add Fairlane challenge selector
* Update DDOS-GUARD title
* Update dependencies

## v3.0.4 (2023/03/07)

* Click on the Cloudflare's 'Verify you are human' button if necessary

## v3.0.3 (2023/03/06)

* Update undetected_chromedriver version to 3.4.6

## v3.0.2 (2023/01/08)

* Detect Cloudflare blocked access
* Check Chrome / Chromium web browser is installed correctly

## v3.0.1 (2023/01/06)

* Kill Chromium processes properly to avoid defunct/zombie processes
* Update undetected-chromedriver
* Disable Zygote sandbox in Chromium browser
* Add more selectors to detect blocked access
* Include procps (ps), curl and vim packages in the Docker image

## v3.0.0 (2023/01/04)

* This is the first release of FlareSolverr v3. There are some breaking changes
* Docker images for linux/386, linux/amd64, linux/arm/v7 and linux/arm64/v8
* Replaced Firefox with Chrome
* Replaced NodeJS / Typescript with Python
* Replaced Puppeter with Selenium
* No binaries for Linux / Windows. You have to use the Docker image or install from Source code
* No proxy support
* No session support

## v2.2.10 (2022/10/22)

* Detect DDoS-Guard through title content

## v2.2.9 (2022/09/25)

* Detect Cloudflare Access Denied
* Commit the complete changelog

## v2.2.8 (2022/09/17)

* Remove 30 s delay and clean legacy code

## v2.2.7 (2022/09/12)

* Temporary fix: add 30s delay
* Update README.md

## v2.2.6 (2022/07/31)

* Fix Cloudflare detection in POST requests

## v2.2.5 (2022/07/30)

* Update GitHub actions to build executables with NodeJs 16
* Update Cloudflare selectors and add HTML samples
* Install Firefox 94 instead of the latest Nightly
* Update dependencies
* Upgrade Puppeteer (#396)

## v2.2.4 (2022/04/17)

* Detect DDoS-Guard challenge

## v2.2.3 (2022/04/16)

* Fix 2000 ms navigation timeout
* Update README.md (libseccomp2 package in Debian)
* Update README.md (clarify proxy parameter) (#307)
* Update NPM dependencies
* Disable Cloudflare ban detection

## v2.2.2 (2022/03/19)

* Fix ban detection. Resolves #330 (#336)

## v2.2.1 (2022/02/06)

* Fix max timeout error in some pages
* Avoid crashing in NodeJS 17 due to Unhandled promise rejection
* Improve proxy validation and debug traces
* Remove @types/puppeteer dependency

## v2.2.0 (2022/01/31)

* Increase default BROWSER_TIMEOUT=40000 (40 seconds)
* Fix Puppeter deprecation warnings
* Update base Docker image Alpine 3.15 / NodeJS 16
* Build precompiled binaries with NodeJS 16
* Update Puppeter and other dependencies
* Add support for Custom CloudFlare challenge
* Add support for DDoS-GUARD challenge

## v2.1.0 (2021/12/12)

* Add aarch64 to user agents to be replaced (#248)
* Fix SOCKSv4 and SOCKSv5 proxy. resolves #214 #220
* Remove redundant JSON key (postData) (#242)
* Make test URL configurable with TEST_URL env var. resolves #240
* Bypass new Cloudflare protection
* Update donation links

## v2.0.2 (2021/10/31)

* Fix SOCKS5 proxy. Resolves #214
* Replace Firefox ERS with a newer version
* Catch startup exceptions and give some advices
* Add env var BROWSER_TIMEOUT for slow systems
* Fix NPM warning in Docker images

## v2.0.1 (2021/10/24)

* Check user home dir before testing web browser installation

## v2.0.0 (2021/10/20)

FlareSolverr 2.0.0 is out with some important changes:

* It is capable of solving the automatic challenges of Cloudflare. CAPTCHAs (hCaptcha) cannot be resolved and the old solvers have been removed.
* The Chrome browser has been replaced by Firefox. This has caused some functionality to be removed. Parameters: `userAgent`, `headers`, `rawHtml` and `downloadare` no longer available.
* Included `proxy` support without user/password credentials. If you are writing your own integration with FlareSolverr, make sure your client uses the same User-Agent header and Proxy that FlareSolverr uses. Those values together with the Cookie are checked and detected by Cloudflare.
* FlareSolverr has been rewritten from scratch. From now on it should be easier to maintain and test.
* If you are using Jackett make sure you have version v0.18.1041 or higher. FlareSolverSharp v2.0.0 is out too.

Complete changelog:

* Bump version 2.0.0
* Set puppeteer timeout half of maxTimeout param. Resolves #180
* Add test for blocked IP
* Avoid reloading the page in case of error
* Improve Cloudflare detection
* Fix version
* Fix browser preferences and proxy
* Fix request.post method and clean error traces
* Use Firefox ESR for Docker images
* Improve Firefox start time and code clean up
* Improve bad request management and tests
* Build native packages with Firefox
* Update readme
* Improve Docker image and clean TODOs
* Add proxy support
* Implement request.post method for Firefox
* Code clean up, remove returnRawHtml, download, headers params
* Remove outdated chaptcha solvers
* Refactor the app to use Express server and Jest for tests
* Fix Cloudflare resolver for Linux ARM builds
* Fix Cloudflare resolver
* Replace Chrome web browser with Firefox
* Remove userAgent parameter since any modification is detected by CF
* Update dependencies
* Remove Puppeter steath plugin

## v1.2.9 (2021/08/01)

* Improve "Execution context was destroyed" error handling
* Implement returnRawHtml parameter. resolves #172 resolves #165
* Capture Docker stop signal. resolves #158
* Reduce Docker image size 20 MB
* Fix page reload after challenge is solved. resolves #162 resolves #143
* Avoid loading images/css/fonts to speed up page load
* Improve Cloudflare IP ban detection
* Fix vulnerabilities

## v1.2.8 (2021/06/01)

* Improve old JS challenge waiting. Resolves #129

## v1.2.7 (2021/06/01)

* Improvements in Cloudflare redirect detection. Resolves #140
* Fix installation instructions

## v1.2.6 (2021/05/30)

* Handle new Cloudflare challenge. Resolves #135 Resolves #134
* Provide reference Systemd unit file. Resolves #72
* Fix EACCES: permission denied, open '/tmp/flaresolverr.txt'. Resolves #120
* Configure timezone with TZ env var. Resolves #109
* Return the redirected URL in the response (#126)
* Show an error in hcaptcha-solver. Resolves #132
* Regenerate package-lock.json lockfileVersion 2
* Update issue template. Resolves #130
* Bump ws from 7.4.1 to 7.4.6 (#137)
* Bump hosted-git-info from 2.8.8 to 2.8.9 (#124)
* Bump lodash from 4.17.20 to 4.17.21 (#125)

## v1.2.5 (2021/04/05)

* Fix memory regression, close test browser
* Fix release-docker GitHub action

## v1.2.4 (2021/04/04)

* Include license in release zips. resolves #75
* Validate Chrome is working at startup
* Speedup Docker image build
* Add health check endpoint
* Update issue template
* Minor improvements in debug traces
* Validate environment variables at startup. resolves #101
* Add FlareSolverr logo. resolves #23

## v1.2.3 (2021/01/10)

* CI/CD: Generate release changelog from commits. resolves #34
* Update README.md
* Add donation links
* Simplify docker-compose.yml
* Allow to configure "none" captcha resolver
* Override docker-compose.yml variables via .env resolves #64 (#66)

## v1.2.2 (2021/01/09)

* Add documentation for precompiled binaries installation
* Add instructions to set environment variables in Windows
* Build Windows and Linux binaries. resolves #18
* Add release badge in the readme
* CI/CD: Generate release changelog from commits. resolves #34
* Add a notice about captcha solvers
* Add Chrome flag --disable-dev-shm-usage to fix crashes. resolves #45
* Fix Docker CLI documentation
* Add traces with captcha solver service. resolves #39
* Improve logic to detect Cloudflare captcha. resolves #48
* Move Cloudflare provider logic to his own class
* Simplify and document the "return only cookies" parameter
* Show message when debug log is enabled
* Update readme to add more clarifications. resolves #53 (#60)
* issue_template: typo fix (#52)

## v1.2.1 (2020/12/20)

* Change version to match release tag / 1.2.0 => v1.2.0
* CI/CD Publish release in GitHub repository. resolves #34
* Add welcome message in / endpoint
* Rewrite request timeout handling (maxTimeout) resolves #42
* Add http status for better logging
* Return an error when no selectors are found, #25
* Add issue template, fix #32
* Moving log.html right after loading the page and add one on reload, fix #30
* Update User-Agent to match chromium version, ref: #15 (#28)
* Update install from source code documentation
* Update readme to add Docker instructions (#20)
* Clean up readme (#19)
* Add docker-compose
* Change default log level to info

## v1.2.0 (2020/12/20)

* Fix User-Agent detected by CouldFlare (Docker ARM) resolves #15
* Include exception message in error response
* CI/CD: Rename GitHub Action build => publish
* Bump version
* Fix TypeScript compilation and bump minor version
* CI/CD: Bump minor version
* CI/CD: Configure GitHub Actions
* CI/CD: Configure GitHub Actions
* CI/CD: Bump minor version
* CI/CD: Configure Build GitHub Action
* CI/CD: Configure AutoTag GitHub Action (#14)
* CI/CD: Build the Docker images with GitHub Actions (#13)
* Update dependencies
* Backport changes from Cloudproxy (#11)
