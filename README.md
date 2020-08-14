# Docker Pull

Docker Hub announced they are going to start purging images, via their new [retention policy](https://www.docker.com/pricing/retentionfaq). 
This is obviously terrible for scientific repodocibility.
This is a simple test to parse container names in [repos.txt](repos.txt) and pull them on a monthly basis.
You should group container repositories together (meaning ones that only vary by the tag)
to ensure that the images are removed after all are pulled (so the GitHub Workflow
space doesn't fill up with the layers).
