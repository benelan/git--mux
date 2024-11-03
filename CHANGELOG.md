# Changelog

## [0.4.0](https://github.com/benelan/git-mux/compare/v0.3.0...v0.4.0) (2024-11-03)


### Features

* Add more detail in error logs ([724f8be](https://github.com/benelan/git-mux/commit/724f8becfd4b6302ef251b09cad498987aa98220))
* Add types and doc via EmmyLua annotations ([99bbbf0](https://github.com/benelan/git-mux/commit/99bbbf0e0953c16bfb59995bcee72ec7cfef07dc))
* Add wezterm support for project command ([8c2c6c5](https://github.com/benelan/git-mux/commit/8c2c6c5366bd1694dd25dfc291cfdc7d07b5cedb))
* Add wezterm support for task command ([e42aef4](https://github.com/benelan/git-mux/commit/e42aef4a9a94d09ab75e82e5b0b40ccfff1b2eea))
* **wezterm:** Improve keybinding functionality ([178731d](https://github.com/benelan/git-mux/commit/178731db86a78c2542a475cc55ff6b79f397ca4a))


### Bug Fixes

* **project:** Properly exit when selection is canceled ([df353ab](https://github.com/benelan/git-mux/commit/df353abc18a1aa1e764456543c3763b0aaba73fc))
* **wezterm:** Fix newline for task command execution ([83448eb](https://github.com/benelan/git-mux/commit/83448ebcc28c036ed8d1c8f890f4dbeda23bc85f))
* **wezterm:** Handle projects with identical task names ([baae236](https://github.com/benelan/git-mux/commit/baae2363c34cbf58b0237c6cf8adce4078793212))

## [0.3.0](https://github.com/benelan/git-mux/compare/v0.2.0...v0.3.0) (2024-05-01)


### Features

* **task:** Sort by commit date during fzf search ([781eb73](https://github.com/benelan/git-mux/commit/781eb73468039ee10adb0ae59592d7a43b39b85d))


### Bug Fixes

* Leading slash in new branch names when PREFIX option unset ([c60989f](https://github.com/benelan/git-mux/commit/c60989f5b82a32f6480e7d0f2d529188b378fa6a))
* Send all messages to stderr ([a161cf6](https://github.com/benelan/git-mux/commit/a161cf68e947ed6bf639425eebd84c40dfb8ced0))

## [0.2.0](https://github.com/benelan/git-mux/compare/v0.1.0...v0.2.0) (2023-12-26)


### Features

* Add option to execute command(s) after creating a new tmux session ([47460b7](https://github.com/benelan/git-mux/commit/47460b738905971832e70c1e858c809bf7467823))
* **clone, project, task:** Add support for long/short flag syntax ([be03324](https://github.com/benelan/git-mux/commit/be033240a7e2c7de6a443a41286fffcf76ff434c))
* **task:** Better error message when a tmux server does not exist ([7a9bee3](https://github.com/benelan/git-mux/commit/7a9bee3670c9b1c8955eee0b84b58a41da00a7a6))


### Bug Fixes

* **project:** Start in the correct directory when a relative path is provided ([f6f8842](https://github.com/benelan/git-mux/commit/f6f88422d3434b1612116979c14c051a5aac8784))

## 0.1.0 (2023-11-28)

### Features

* Add better help/error messages and make sure they go to stderr ([e2dd3c5](https://github.com/benelan/git-mux/commit/e2dd3c5fd89258f677cb0f79cb8f83695b24167a))
* Add `$GIT_MUX_LOG_LEVEL` config option to only save logs for certain levels ([bd0583b](https://github.com/benelan/git-mux/commit/bd0583b6a140a7fc6dce7bb91d8bcf431533b99c))
* Combine directories specified in `$GIT_MUX_PROJECTS` and `$GIT_MUX_PROJECT_PARENTS` config options ([b33aacf](https://github.com/benelan/git-mux/commit/b33aacfe974140b7f5115387d9fb03827793a1ee))
* And `$GIT_MUX_NEW_WORKTREE_CMD` config option for executing a command in git worktrees after they are created ([2395cc2](https://github.com/benelan/git-mux/commit/2395cc2fc1ea43ea3ebd61a06de0e005f283dec3)), ([7dc1af7](https://github.com/benelan/git-mux/commit/7dc1af78b2bf8b4c061c741a5f580b1300252de3))

### Bug Fixes

* Log level off by one error ([9960fe6](https://github.com/benelan/git-mux/commit/9960fe6c660afd56f3c1b7e378072173a25c75c4))
* **task**: Only add branch prefix if one doesn't exist ([097c6e2](https://github.com/benelan/git-mux/commit/097c6e2033fc2be2e765428b4fff0af3ac8cf5e4))
* Prevent trying to write to a nonexistent log file ([c375081](https://github.com/benelan/git-mux/commit/c3750814ee89791575666d849f8aaf6261720d1e))
* **task:** Remove trailing space in tmux window name for new git tasks ([00b911d](https://github.com/benelan/git-mux/commit/00b911d4a13639b151c8def1d90af18413b5b851))
* **project:** Attach to existing tmux session if it exists ([f646543](https://github.com/benelan/git-mux/commit/f6465436b79bb967e30f07c39d3ab13074cc1e7d))
* **project:** Fallback to creating the tmux session in `$HOME` if the path argument is not provided ([26d6165](https://github.com/benelan/git-mux/commit/26d61659ea20d75e921fc735df265f2f5df60843))
* Stop exiting early when checking log level ([9df85b5](https://github.com/benelan/git-mux/commit/9df85b5f481deea5bf9df8507052c5c8f9b7f239))
* **task:** Stop combining multiple arguments into a single string ([7fbf5f3](https://github.com/benelan/git-mux/commit/7fbf5f3369cba27ee1098a94ff55ade58b33b9dc))
* **task:** Change `tmux new-window` command options for backwards compatibility ([fcf36f7](https://github.com/benelan/git-mux/commit/fcf36f7bcc882c8629f4f249fd1af956a9237b75))
