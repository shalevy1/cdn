# cdn
My CDN file for jsdelivr

# https://medium.com/javarevisited/how-to-host-your-repository-js-css-on-open-source-cdn-jsdelivr-4de252d6fbad

jsDelivr CDN over GitHub Assets
jsDelivr does exactly what many of us need, provides a opensource cdn over github assets. Let look into it in detail.

Here’s how it works.

jsDelivr CDN service’s base URL is https://cdn.jsdelivr.net/gh/{username}/{repo}/, where you replace {username} with the GitHub username and {repo} with the repository name for the project.
Append that URL with the path to the file you want to access in the project. For example, consider my sample project Github-As-CDN , the JavaScript file(dummy-js-file.js) is located in the /dist directory.
<html>
...
...
<script src="https://cdn.jsdelivr.net/gh/root0109/github-cdn/dist/dummy-js-file.js"></script>
...
...
</html>
You can also take advantage of semantic versioning by adding @{version-number} to the repository name. You can target major, minor, and patch releases as desired.

https://cdn.jsdelivr.net/gh/shalevy1/cdn/dist/dummy-js-file.js
