# chart-test
testing a helm chart issue

## Current issue

I'm currently getting this output when I `helm lint`:

```
$ helm lint .
dependencies.go:260: Warning: ImportValues missing table: "helmet" is not a table
==> Linting .
[ERROR] templates/: template: test-parent/charts/test-child/templates/app.yaml:1:3: executing "test-parent/charts/test-child/templates/app.yaml" at <include "helmet.app" .>: error calling include: template: no template "helmet.app" associated with template "gotpl"

Error: 1 chart(s) linted, 1 chart(s) failed
```

I'm really not sure what I'm missing...
