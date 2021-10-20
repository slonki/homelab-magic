
# Guidelines for contributing

---

## Steps to contribute

1. Create an issue
* The issue needs to clearly explain what your contribution will be.

2. Request the issue to be assigned to you
* Leave a comment on the issue, and a maintainer will assign it.

4. Fork the repo and commit your work

5. Create a Pull Request
* The PR will be reviewed by a maintainer and approved/declined based on its contents.

## Requirements to contribute
### The issue must be assigned to you
Since the repo is currently enrolled in the hacktoberfest project, an issue needs to be created and contributors need to request to work on it for the PRs to be approved.



### Code must be commented

The comments do not need to be extensive, but anyone, including those who do not know the language, should have a general understanding of what the code does based on the comments.

Examples:
* Comment that can be improved:
``` 
# Check arguments
if [[ $# -eq 0 ]]; then
echo  "Example output"
exit 1
fi
```
* Good comment:
```
# Handle 0 arguments given
if [[ $# -eq 0 ]]; then 
echo  "Example output"
exit 1
fi
```

### Projects must be put in their own directories
When creating a new file, it should be put into its own subdirectory within the appropriate directory.

### Documentation must be created
Alongside your contribution, a .md file needs to be created explaining what it does, how it does it (in case necessary), and an example for how to use it.

### Be nice!
This repo is here to help people set up their homelab as easily as possible. Be friendly and polite to everyone,  and have fun!