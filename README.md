<h1>Installation Steps:</h1>

1. Clone the repository
2. Save **branch-switch** file to a directory in your PATH, e.g., **/usr/local/bin**<br>
   `sudo cp branch-switch /usr/local/bin/branch-switch`
3. Make it executable<br>
   `sudo chmod +x /usr/local/bin/branch-switch`

<h1>Configuration:</h1>

1. **Create configuration file:**<br>
   `branch-switch --config`
2. **Add your aliases** to the config file. Format:<br>
   `/full/path/to/directory:alias_name:actual_branch_name`<br>
   Example:<br>
   ```
   /home/user/my_project:prod:prod_branch
   /home/user/my_project:dev:development_branch
   /home/user/my_project:staging:staging_branch
   /home/user/another_project:main:master
   ```

<h1>Usage Examples:</h1>

- Basic branch switching<br>
  `branch-switch main`
- Switch with alias (if configured)<br>
  `branch-switch prod`
- Switch and pull<br>
  `branch-switch prod --pull`
- List configured aliases for current directory<br>
  `branch-switch --list`
- Open configuration file<br>
  `branch-switch --config`
- Show help<br>
  `branch-switch --help`
