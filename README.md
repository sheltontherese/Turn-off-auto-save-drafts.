# Turn-off-auto-save-drafts.
Turn off auto-save drafts.
// Disable post autosave
add_action('wp_print_scripts', 'disable_autosave');
function disable_autosave()
{
    wp_deregister_script('autosave');
}
