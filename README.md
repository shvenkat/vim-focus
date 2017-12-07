Focus on content by reducing visual distractions.

# SUMMARY

This plugin was inspired by Junegunn Choi's goyo.vim. goyo.vim creates a new tab
with a single _visible_ window showing just the buffer, with all margin
annotations hidden. I found that preferred to have an inconspicuous view of
certain annotations such as line number, gitgutter and neomake annotations.
focus updates the color scheme and margin settings to do just this in the
current tab and window.

# BUGS

Split windows are not well supported. The plugin tracks a global focus state
rather than one per window. It works best if focus mode is first enabled, and
then the windows are split as needed. And conversely, if all but one windows are
closed before disabling focus mode. It's not clear if there can be a per-window
focus state, because colorscheme is global and cannot be set per window.
