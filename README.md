curl -L \
  -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/repos/OWNER/REPO/security-advisories/reports \
  -d '{"summary":"A newly discovered vulnerability","description":"A more in-depth description of what the problem is.","severity":"high","vulnerabilities":[{"package":{"name":"a-package","ecosystem":"npm"},"vulnerable_version_range":"< 1.0.0","patched_versions":"1.0.0","vulnerable_functions":["important_function"]}],"cwe_ids":["CWE-123"]}'
