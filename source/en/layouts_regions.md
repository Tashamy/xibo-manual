<!--toc=layouts-->

# Regions (New Features for v2)

Regions define areas on a **Layout** which hold **Widgets** (media content) to form sets of timed content.

{tip}
If you are using 1.8 please use the following link to the appropriate manual page for your version: [Regions 1.8](layouts_regions_1.8.html)
{/tip}

{tip}
A new Layout will contain one full size empty **Region** by default ready for resizing, positioning and adding media content to. 

Ensure that the Layout has been 'checked out' to enable editing.
{/tip}

Click on the 'edit' icon located in the top right hand corner of the **Layout Navigator** window to open.

**Regions** can be positioned anywhere inside the **Layout** canvas using drag and drop, and resized by using the resize handle located in the lower right-hand corner of the Region. 

Click in the Region to resize and position, further actions are available via the tabs on the **Region Options** form.

![Region Resize](img/v2_layouts_regions_resize.png)



## Region Options

### General

Complete a name for the Region and use the checkbox to Loop the content if required.

### Positioning

This tab allows for precise sizing and positioning as well as setting a **Layering Order**.  **Make the Region full screen** by clicking on the text which will display the dimensions the Region will be set by.

### Rules for Layering Regions

**Please note: Overlapping Regions is not supported for Windows Players.**

If required, overlapping Regions can be ordered for playback using z-index settings.

These are set from the **Positioning Tab**, by entering a number in the **Layer** field to determine the order that Region should be shown within the overall stack.

![Region Options Layering](img/v2_layouts_regions_layer.png)

The ‘Layer’ order is determined by the number entered here, with 1 considered the lowest Layer. The higher the number the higher the Layer.

{tip}
On some devices, it is impossible to overlay anything on a Region showing a **Video** or **VideoIn** Widget. Whether it is possible will depend on the device and whether hardware accelerated playback is being used. In general, it is possible on Android (when not using the SurfaceView option in the Display Settings Profile), Linux, Tizen and webOS Players, but if you have a requirement for this, be sure to test your intended device carefully to ensure this works in your use case.
{/tip}

### Transition

**Exit Transitions** happen when the last media item in a Region is shown and occurs only when all other media items have expired in the other Regions. 

{tip}
Transitions are only supported in the Linux, Android and webOS Players and need to be pre configured. Please contact your Administrator.
{/tip}

Once you have **Saved** your edits click **Close** to return to the Layout Designer screen.

![Resized Region Layout Navigator](img/v2_layouts_regions_resized_layout_navigator.png)



## Adding Regions

Regions can be added in two ways:

- open the **Layout Navigator** window and click on the **Add Region** button.![Add Region Button](img/v2_layouts_regions_add_button.png)

- select **Tools** on the bottom toolbar and click on **Region** to add or drag to the Layout Navigator window.![Add Region](img/v2_layouts_regions_add.png)


### Deleting Regions

Remove Regions and all associated content by clicking on the **Delete Region** button in the Layout Navigator window. **Please note: This action cannot be undone**.

{tip}
Regions can be deleted from the Layout Designer by clicking on the Region and clicking the bin icon on the bottom toolbar or by right clicking on the target Region and using the bin icon.
{/tip}

### Permissions for a Region

Control which **User** and **User Groups** can view/edit/delete the Region.  Click on the **Permissions** button, located under **Tools** on the toolbar then click or drag to the target Region. Edit the Permissions form as appropriate.

{tip}
Assign/Edit permissions by right clicking on the target Region.
{/tip}

**Please note:** The owner of the Layout has full control over sharing. 

{tip}
A globally shared Layout can have Region access rights defined for any other users of the CMS. Read more for [Permissions for User Objects](users_permissions.html#user_objects) 
{/tip}

{tip}
**Please note:** The Windows Player does not support overlapping Regions. For a mixed Player network ensure Regions do not overlap for the best results.
{/tip}



