# Vue v3 devtools v-if issue

## Issue
`v-if` disables component creation, until the expression is true. A component that's not created should not turn op in
the devtools. But when the `v-if` expression changes value, the devtools Inspector should update.

## Credits
This repo was created by this vue v3 template repo: https://github.com/blacksonic/vue-3-playground.


