# Mobillium Project Guidelines

Project & code-style guideline of Mobillium Android Development Team.

## Resources Naming Standarts

**Strings.xml**

    lowercase_underscore

| Rule | Definition | Example | Common
|--|--|--|--|
| `<where>_screen_<description>_<type>` <br> or <br> `<where>_<description>_<type>` | **where** = DieticianDetailActivity + *screen* <br> **description** = Credit card type <br> **type** = Header  | dietician_detail_screen_credit_card_type_header | common_loading


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
