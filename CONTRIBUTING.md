Every PR should start with:

```
| Q                    | A
| -------------------- | ---
| Specs pass?*         |
| Checkstyle issues?** |
| PMD issues?***       | 
| Changelog updated?   |
| Fixed tickets        |
```

*``` > ./bin/phpspec run```
**``` > ./bin/phpcs --standard=PSR2 --extensions=php ./```
***``` > ./bin/phpmd ./ text cleancode,codesize,controversial,design,naming,unusedcode --strict --exclude vendor

Check that each commit should start by the JIRA ticket code
Same for your PR name
