# How to show a border around a focused editor


<p>This example shows the way to change the visual appearance of a focused editor.</p>
<p>Let's assume that the editor must show an additional border when focused.</p>
<p>To create this feature, it's necessary to create a custom template and place a new border element there, which will be displayed every time the control is focused. There is a template "WPFEditorsFocusFrame" in the resource dictionary in which rectangle named "FocusFrame" is defined. This rectangle is playing the role of the focus border, and it's Visibility property is bound to the IsKeyboardFocusWithin property of the control.</p>
<p>The described template is general for several DXEditors types and is applied automatically to TextEdit, PasswordBoxEdit, ButtonEdit, ComboBoxEdit, LookupEdit and other button-based editors. So, once you define this template, you'll get the same behavior for all of these controls.<br><br></p>
<p><strong>Starting with version 16.1</strong>, we changed our templates and introduced the new default theme - Office2016White. So, you need to use the HoverBorderTemplate resource to accomplish this task.</p>

<br/>


