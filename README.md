<!-- Generated with Stardoc: http://skydoc.bazel.build -->

# A Bazel test rule for text files.
## `MODULE.bazel`

```
bazel_dep(
    name = "com_github_bcsgh_text_tools",
    version = ...,
)
```

<a id="spell_test"></a>

## spell_test

<pre>
load("@com_github_bcsgh_text_tools//text:spelling.bzl", "spell_test")

spell_test(<a href="#spell_test-name">name</a>, <a href="#spell_test-dict">dict</a>, <a href="#spell_test-file">file</a>)
</pre>

Spell check a text file.

NOTE: this requiers that 'spell' be installed on the build system:

sudo apt install spell  # or the equivlent.

**ATTRIBUTES**


| Name  | Description | Type | Mandatory | Default |
| :------------- | :------------- | :------------- | :------------- | :------------- |
| <a id="spell_test-name"></a>name |  A unique name for this target.   | <a href="https://bazel.build/concepts/labels#target-names">Name</a> | required |  |
| <a id="spell_test-dict"></a>dict |  A list of supplemental dictionaries to merge and use.   | <a href="https://bazel.build/concepts/labels">List of labels</a> | optional |  `[]`  |
| <a id="spell_test-file"></a>file |  The file to spell check.   | <a href="https://bazel.build/concepts/labels">Label</a> | required |  |

## Setup (for development)
To configure the git hooks, run `./.git_hooks/setup.sh`
