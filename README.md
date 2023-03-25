## The Beginning

This `.eslintrc.json` provides reasonable and strict code checking, as well as excellent readability style checking.

However, due to the inability of `ESLint` + `typescript-eslint` + `Prettier` combination to simultaneously consider performance, scalability, and ease of use, I no longer plan to use you.

Next, I plan to use [`Rome`](https://rome.tools/).

<br/>

## The Turning Point

I have decided to switch back to using `ESLint` + `typescript-eslint` because `Rome` does not allow for custom code styles (everything else is great). 

> 👀 Suddenly, I realized that I should create a `create-jynxio-app` project.

<br/>

<br/>

## Version

``` json
"eslint": "^8.36.0"
```

<br/>

## .eslintrc.json

``` json
{
	"root": true,
	"env": { "es2022": true, "browser": true, "node": true, "worker": true },
	"overrides": [],
	"extends": [ "eslint:recommended" ],
	"parserOptions": { "ecmaVersion": "latest", "sourceType": "module" },
	"parser": "@typescript-eslint/parser",
	"plugins": [ "@typescript-eslint" ],
	"noInlineConfig": true,
	"rules": {
		"indent": [
			"error",
			"tab",
			{
				"ignoredNodes": [
					"ConditionalExpression"
				]
			}
		],
		"linebreak-style": [
			"error",
			"unix"
		],
		"quotes": [
			"error",
			"double"
		],
		"semi": [
			"error",
			"always"
		],
		"camelcase": [
			"error"
		],
		"capitalized-comments": [
			"error",
			"always",
			{
				"ignoreInlineComments": true,
				"ignoreConsecutiveComments": true
			}
		],
		"curly": [
			"error",
			"multi",
			"consistent"
		],
		"consistent-this": [
			"error",
			"that"
		],
		"default-param-last": [
			"error"
		],
		"dot-notation": [
			"error"
		],
		"default-case-last": [
			"error"
		],
		"func-name-matching": [
			"error"
		],
		"func-names": [
			"error",
			"as-needed"
		],
		"func-style": [
			"error",
			"declaration",
			{
				"allowArrowFunctions": true
			}
		],
		"grouped-accessor-pairs": [
			"error",
			"getBeforeSet"
		],
		"max-depth": [
			"error",
			3
		],
		"max-nested-callbacks": [
			"error",
			3
		],
		"max-params": [
			"error",
			3
		],
		"multiline-comment-style": [
			"error",
			"starred-block"
		],
		"new-cap": [
			"error"
		],
		"no-alert": [
			"error"
		],
		"no-floating-decimal": [
			"error"
		],
		"no-implicit-coercion": [
			"error"
		],
		"no-implied-eval": [
			"error"
		],
		"no-iterator": [
			"error"
		],
		"no-lone-blocks": [
			"error"
		],
		"no-lonely-if": [
			"error"
		],
		"no-multi-str": [
			"error"
		],
		"no-negated-condition": [
			"error"
		],
		"no-new": [
			"error"
		],
		"no-new-func": [
			"error"
		],
		"no-new-object": [
			"error"
		],
		"no-new-wrappers": [
			"error"
		],
		"no-octal-escape": [
			"error"
		],
		"no-param-reassign": [
			"error"
		],
		"no-proto": [
			"error"
		],
		"no-return-await": [
			"error"
		],
		"no-throw-literal": [
			"error"
		],
		"no-undef-init": [
			"error"
		],
		"no-undefined": [
			"error"
		],
		"no-underscore-dangle": [
			"error",
			{
				"enforceInMethodNames": true,
				"enforceInClassFields": true,
				"allowInArrayDestructuring": false,
				"allowInObjectDestructuring": false
			}
		],
		"no-unneeded-ternary": [
			"error"
		],
		"no-useless-call": [
			"error"
		],
		"no-useless-computed-key": [
			"error",
			{
				"enforceForClassMembers": true
			}
		],
		"no-useless-concat": [
			"error"
		],
		"no-useless-constructor": [
			"error"
		],
		"no-useless-return": [
			"error"
		],
		"no-var": [
			"error"
		],
		"prefer-exponentiation-operator": [
			"error"
		],
		"prefer-object-has-own": [
			"error"
		],
		"prefer-object-spread": [
			"error"
		],
		"prefer-promise-reject-errors": [
			"error"
		],
		"prefer-rest-params": [
			"error"
		],
		"prefer-spread": [
			"error"
		],
		"require-await": [
			"error"
		],
		"radix": [
			"error"
		],
		"sort-imports": [
			"error",
			{
				"memberSyntaxSortOrder": [
					"none",
					"all",
					"single",
					"multiple"
				],
				"allowSeparatedGroups": true
			}
		],
		"spaced-comment": [
			"error"
		],
		"symbol-description": [
			"error"
		],
		"array-bracket-newline": [
			"error",
			"consistent"
		],
		"array-bracket-spacing": [
			"error",
			"always"
		],
		"arrow-parens": [
			"error",
			"as-needed"
		],
		"no-unused-vars": [
			"error",
			{
				"vars": "all",
				"args": "none",
				"caughtErrors": "all",
				"argsIgnorePattern": "_$",
				"caughtErrorsIgnorePattern": "^_$"
			}
		],
		"arrow-spacing": [
			"error"
		],
		"block-spacing": [
			"error"
		],
		"brace-style": [
			"error"
		],
		"comma-dangle": [
			"error",
			{
				"arrays": "always-multiline",
				"objects": "always-multiline",
				"imports": "always-multiline",
				"exports": "always-multiline",
				"functions": "always-multiline"
			}
		],
		"comma-spacing": [
			"error"
		],
		"comma-style": [
			"error"
		],
		"computed-property-spacing": [
			"error",
			"always",
			{
				"enforceForClassMembers": true
			}
		],
		"dot-location": [
			"error",
			"property"
		],
		"eol-last": [
			"error",
			"always"
		],
		"func-call-spacing": [
			"error"
		],
		"function-call-argument-newline": [
			"error",
			"consistent"
		],
		"function-paren-newline": [
			"error",
			"multiline"
		],
		"generator-star-spacing": [
			"error",
			{
				"before": false,
				"after": true
			}
		],
		"implicit-arrow-linebreak": [
			"error"
		],
		"jsx-quotes": [
			"error"
		],
		"key-spacing": [
			"error"
		],
		"keyword-spacing": [
			"error"
		],
		"lines-around-comment": [
			"error",
			{
				"beforeBlockComment": true,
				"beforeLineComment": true,
				"allowBlockStart": false,
				"allowBlockEnd": false,
				"allowClassStart": false,
				"allowClassEnd": false,
				"allowObjectStart": true,
				"allowObjectEnd": true,
				"allowArrayStart": true,
				"allowArrayEnd": true
			}
		],
		"lines-between-class-members": [
			"error"
		],
		"max-len": [
			"error",
			{
				"code": 100,
				"tabWidth": 4,
				"comments": 100,
				"ignoreTrailingComments": false,
				"ignoreUrls": true,
				"ignoreStrings": true,
				"ignoreTemplateLiterals": true,
				"ignoreRegExpLiterals": true
			}
		],
		"operator-linebreak": [
			"error",
			"before",
			{
				"overrides": {
					"?": "none",
					":": "before"
				}
			}
		],
		"new-parens": [
			"error",
			"always"
		],
		"no-multi-spaces": [
			"error",
			{
				"ignoreEOLComments": true
			}
		],
		"no-multiple-empty-lines": [
			"error",
			{
				"max": 1,
				"maxEOF": 0,
				"maxBOF": 0
			}
		],
		"no-tabs": [
			"error",
			{
				"allowIndentationTabs": true
			}
		],
		"no-trailing-spaces": [
			"error"
		],
		"no-whitespace-before-property": [
			"error"
		],
		"nonblock-statement-body-position": [
			"error"
		],
		"object-curly-newline": [
			"error",
			{
				"ObjectExpression": {
					"consistent": true
				},
				"ObjectPattern": {
					"consistent": true
				},
				"ImportDeclaration": {
					"consistent": true
				},
				"ExportDeclaration": {
					"consistent": true
				}
			}
		],
		"object-curly-spacing": [
			"error",
			"always",
			{
				"arraysInObjects": true,
				"objectsInObjects": true
			}
		],
		"padded-blocks": [
			"error"
		],
		"padding-line-between-statements": [
			"error",
			{
				"blankLine": "always",
				"prev": "*",
				"next": "block"
			},
			{
				"blankLine": "always",
				"prev": "block",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "block-like"
			},
			{
				"blankLine": "always",
				"prev": "block-like",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "break"
			},
			{
				"blankLine": "always",
				"prev": "break",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "case"
			},
			{
				"blankLine": "always",
				"prev": "case",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "cjs-export"
			},
			{
				"blankLine": "always",
				"prev": "cjs-export",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "cjs-export",
				"next": "cjs-export"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "cjs-import"
			},
			{
				"blankLine": "always",
				"prev": "cjs-import",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "cjs-import",
				"next": "cjs-import"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "class"
			},
			{
				"blankLine": "always",
				"prev": "class",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "const"
			},
			{
				"blankLine": "always",
				"prev": "const",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "const",
				"next": "const"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "continue"
			},
			{
				"blankLine": "always",
				"prev": "continue",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "debugger"
			},
			{
				"blankLine": "always",
				"prev": "debugger",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "default"
			},
			{
				"blankLine": "always",
				"prev": "default",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "directive"
			},
			{
				"blankLine": "always",
				"prev": "directive",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "do"
			},
			{
				"blankLine": "always",
				"prev": "do",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "export"
			},
			{
				"blankLine": "always",
				"prev": "export",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "export",
				"next": "export"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "expression"
			},
			{
				"blankLine": "always",
				"prev": "expression",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "expression",
				"next": "expression"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "for"
			},
			{
				"blankLine": "always",
				"prev": "for",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "if"
			},
			{
				"blankLine": "always",
				"prev": "if",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "iife"
			},
			{
				"blankLine": "always",
				"prev": "iife",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "import"
			},
			{
				"blankLine": "always",
				"prev": "import",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "import",
				"next": "import"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "let"
			},
			{
				"blankLine": "always",
				"prev": "let",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "let",
				"next": "let"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "return"
			},
			{
				"blankLine": "always",
				"prev": "return",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "switch"
			},
			{
				"blankLine": "always",
				"prev": "switch",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "throw"
			},
			{
				"blankLine": "always",
				"prev": "throw",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "try"
			},
			{
				"blankLine": "always",
				"prev": "try",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "var"
			},
			{
				"blankLine": "always",
				"prev": "var",
				"next": "*"
			},
			{
				"blankLine": "any",
				"prev": "var",
				"next": "var"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "while"
			},
			{
				"blankLine": "always",
				"prev": "while",
				"next": "*"
			},
			{
				"blankLine": "always",
				"prev": "*",
				"next": "with"
			},
			{
				"blankLine": "always",
				"prev": "with",
				"next": "*"
			}
		],
		"semi-spacing": [
			"error"
		],
		"semi-style": [
			"error"
		],
		"space-before-blocks": [
			"error"
		],
		"space-before-function-paren": [
			"error"
		],
		"space-in-parens": [
			"error",
			"always"
		],
		"space-infix-ops": [
			"error"
		],
		"space-unary-ops": [
			"error",
			{
				"words": true,
				"nonwords": true
			}
		],
		"switch-colon-spacing": [
			"error"
		],
		"template-curly-spacing": [
			"error",
			"always"
		],
		"template-tag-spacing": [
			"error",
			"always"
		],
		"wrap-iife": [
			"error",
			"inside"
		],
		"wrap-regex": [
			"error"
		],
		"yield-star-spacing": [
			"error",
			"after"
		],
		"line-comment-position": [
			"error",
			"beside"
		],
		"array-callback-return": [
			"error"
		],
		"no-await-in-loop": [
			"error"
		],
		"no-constant-binary-expression": [
			"error"
		],
		"no-constructor-return": [
			"error"
		],
		"no-duplicate-imports": [
			"error",
			{
				"includeExports": true
			}
		],
		"no-new-native-nonconstructor": [
			"error"
		],
		"no-promise-executor-return": [
			"error"
		],
		"no-self-compare": [
			"error"
		],
		"no-template-curly-in-string": [
			"error"
		],
		"no-unmodified-loop-condition": [
			"error"
		],
		"no-unused-private-class-members": [
			"error"
		],
		"accessor-pairs": [
			"error",
			{
				"getWithoutSet": true,
				"setWithoutGet": true,
				"enforceForClassMembers": true
			}
		],
		"block-scoped-var": [
			"error"
		],
		"class-methods-use-this": [
			"error"
		],
		"consistent-return": [
			"error"
		],
		"default-case": [
			"error"
		],
		"eqeqeq": [
			"error",
			"always"
		],
		"guard-for-in": [
			"error"
		],
		"no-array-constructor": [
			"error"
		],
		"no-empty-static-block": [
			"error"
		],
		"no-eval": [
			"error"
		],
		"no-extra-bind": [
			"error"
		],
		"no-extra-label": [
			"error"
		],
		"no-invalid-this": [
			"error"
		],
		"no-loop-func": [
			"error"
		]
	}
}
```
