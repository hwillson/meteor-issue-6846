# meteor-issue-6846

Reproduction for [https://github.com/meteor/meteor/issues/6846](https://github.com/meteor/meteor/issues/6846).

The [Importing styles from npm](https://guide.meteor.com/using-npm-packages.html#npm-styles) 
section of the Meteor Guide seems to imply that importing `.css` files from npm 
packages, using the CSS `@import` syntax, should be supported. This 
reproduction shows that it does not work using either of the following 
syntax approaches:

```
@import '{}/node_modules/normalize.css/normalize.css';
@import '../node_modules/normalize.css/normalize.css';
```

## Steps

1. `git clone https://github.com/hwillson/meteor-issue-6846.git`
2. `cd meteor-issue-6846`
3. `meteor npm install`
4. `meteor`
5. Access http://localhost:3000/

