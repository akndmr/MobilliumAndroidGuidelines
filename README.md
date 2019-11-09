# Mobillium Project Guidelines

Project & code-style guideline of Mobillium Android Development Team.

## Resources Naming Standarts

**Strings.xml**

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `<where>_screen_<description>_<type>` <br> or <br> `<where>_<description>_<type>` <br> or <br> `common_<description>`| **where** = DieticianDetailActivity + *screen* <br> **description** = Credit card type <br> **type** = Header  | `dietician_detail_screen_credit_card_type_header` <br> `common_loading`|


<br>

**Text Sizes**

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `text_size_<description>`  | **description** = caption, small, medium, normal, big, headline |  `text_size_caption = 12sp` 

<br>

**Styles**

    PascalCase

| Rule | Definition | Example
|--|--|--|
| `<Widget><Description>`<br> or <br> `<Where><Description>` | For header texts| `name="TextHeader" parent="Widget.AppCompat.TextView"` |
|`<Widget><Description>.<Style>`| Extends all styles from TextHeader and adds new color style | `name="TextHeader.Black"` |

<br>

**Colors** 

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `<widget/where>_<description>`| **widget/where** =  widget name or where it's used | `<color name="image_logo_tint">@color/mobillium_blue</color>` <br> `<color name="button_primary">@color/pistachio</color>`<br> `<color name="mobillium_blue">#4b7bec</color>`<br> `<color name="pistachio">#93c572</color>`

<br>

**Dimension**

    lowercase_underscore
| Rule | Definition | Example
|--|--|--|
| `<where>_screen_<widget>_<description>` <br> or <br> `<where>_<widget>_<description>` <br> or <br>`<widget>_<description>` <br> or <br> `<attribute>_<description>` | **where** =  where it's used(activity,fragment,dialog) <br> **widget** = widget name(button, image etc) <br> **attribute** = margin, padding | `<dimen name="user_detail_screen_cardview_radius">4dp</dimen>`  <br> `<dimen name="dialog_icon_height">16dp</dimen>` <br> `<dimen name="image_width">120dp</dimen>` <br> `<dimen name="margin_medium">16dp</dimen>`|

