# ALXprodev-advanced_git
Educational: In this project, I practice basic git flow using the proposed technique by Vincent Driessen

## NOTE
The installation possesses certain challenges because of the following issues:
- Git protocol issue: The git:// protocol is often blocked by firewalls/networks
- Missing make command: You're on Windows (Git Bash) which doesn't have make by default

## INSTALLATION FIX
```bash
# Configure git to use HTTPS instead of git://
git config --global url."https://github.com/".insteadOf git://github.com/

# Now try cloning again
cd ~
rm -rf gitflow  # Remove the incomplete clone
git clone --recursive https://github.com/nvie/gitflow.git
```

You might face an issue with the above bash command especially if you had attempted to install it earlier. Solve this by removing the initial installation that might be broken or incomplete with the command below:

```bash
sudo rm -r ~/gitflow
```