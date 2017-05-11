# Angular $http .success()/.failure() transform
Codemod to convert $http `.success()`/`.failure()` methods to `.then(success, failure)` (breaking change in Angular 1.6)
See https://github.com/angular/angular.js/commit/b54a39e2029005e0572fbd2ac0e8f6a4e5d69014

## Setup
 * Install jscodeshift (https://github.com/facebook/jscodeshift#install)
    ```
    npm install -g jscodeshift
    ```

## Run
```
jscodeshift path/to/source/files/ -t path/to/angular-http-success-failure-transform.js
```

## License

MIT
