### Description:

The Link Widget module provides a elegant way for wrapping an link around a
"image" or "text" field type output. This module is dependent upon the [Field
Widget Storage API](https://drupal.org/sandbox/droath/1992692), which provides
a solution for saving extra widget configurations alongside a field.

### What are the differences between Link Widget and related link modules?

The biggest difference is based on the modules architect; instead of creating
another field type, I just created a field widget that extends the field
configurations. You can make either an image or text field type linkable. This
concept can be extended and can accommodate for other field types in future
releases.

### What are the advantages of the Link Widget module?

There are a couple advantages of the Link Widget module. First and foremost,
there is less code to maintain. As I'm only defining a field widget, and don't
have to worry about recreating the field component. Second, the Link Widget is
flexible and making a text or image field linkable, is super easy and can be
done by just selecting a field widget type "Link".

### What link attributes does Link Widget module support?

  * Class - Specifies one or more class names for an element.
  * Rel - Specifies the relationship between the current document and the linked document.
  * Target - Specifies where to open the linked document.
  * Media - Specifies what media/device the linked document is optimized for.
  * Type - Specifies the MIME type of the linked document.

**Note:** I exposed a drupal hook so other modules can add their own attributes.

#### Supported Modules:

  * [FlexSlider 7.x-1.x](https://drupal.org/project/flexslider)
  * [Token](https://drupal.org/project/token)

#### Related Modules:

  * [Link](https://drupal.org/project/link)
  * [Link Image Field](https://drupal.org/project/linkimagefield)

#### Dependencies:

  * [Field Widget Storage API](https://github.com/droath/Field-Widget-Storage-API)

