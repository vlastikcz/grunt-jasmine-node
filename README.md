# @vlastikcz/grunt-jasmine-node
This is fork of [grunt-jasmine-node](https://github.com/jasmine-contrib/grunt-jasmine-node), which seems not to be maintained anymore. 

The goal of this is to fix **outdated and vulnerable dependencies**, not to develop any new features or fix other non-security bugs.

> No new packages should use this library, it's a temporary solution for legacy applications which are not ready to use another library yet. 

# grunt-jasmine-node
A grunt.js task to run your jasmine feature suite using jasmine-node.

## Getting Started
Install this grunt plugin next to your project's grunt.js gruntfile with: `npm install grunt-jasmine-node`

Then add this line to your project's `grunt.js` grunt file:

```javascript
grunt.initConfig({
  jasmine_node: {
    options: {
      forceExit: true,
      match: '.',
      matchall: false,
      extensions: 'js',
      specNameMatcher: 'spec'
    },
    all: ['spec/']
  }
});

grunt.loadNpmTasks('grunt-jasmine-node');

grunt.registerTask('default', 'jasmine_node');
```

## Bugs

Help us squash them by submitting an issue that describes how you encountered it; please be as specific as possible including operating system, node, grunt, and grunt-jasmine-node versions.

## Release History

see [GitHub Repository](/vlastikcz/grunt-jasmine-node).

## License
Licensed under the MIT license.
