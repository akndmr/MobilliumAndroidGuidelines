![Mobillium logo](http://mobillium.com/assets/images/logo.png)
# Mobillium Project Guidelines

Project & code-style guideline of Mobillium Android Development Team.

## Table of Contents

[Colors](#colors) <br>
[CustomViews & CustomLayouts](#customviews-and-customlayouts) <br>
[Dimens](#dimens) <br>
[ID's in XML](#ids-in-xml) <br>
[Resources](#resources) <br>
[Strings](#stringsxml) <br>
[Styles](#styles) <br>
[Text Sizes](#text-sizes) <br>

## 📃Resources Naming Standarts

### 🔸Colors

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `<widget/where>_<description>_<alpha>`| **widget/where** =  widget name or where it's used <br> **alpha** = Transparency percentage (CC000000 - 80% black transparent)| ◾`<color name="image_logo_tint">@color/mobillium_blue</color>` <br> ◾`<color name="button_primary">@color/pistachio</color>`<br> ◾`<color name="button_inactive">@color/iron_80</color>`<br> ◾`<color name="mobillium_blue">#4b7bec</color>`<br> ◾`<color name="pistachio">#93c572</color>`<br> ◾`<color name="iron_80">#CC48494B</color>`

<br>

### 🔸CustomViews and CustomLayouts

    Class: PascalCase, Layout: lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `CV<What><Type>` | **What** = Name for the custom view <br> **Type** = Usually, what it extends | ◾`CVPinTextView`<br> ◾`CVNumPadLayout` |
| `cv_<what>_<type>` | Layout file of custom view or layout | ◾`cv_pin_textview` <br> ◾`cv_numpad_layout` |

<br>

### 🔸Dimens

    lowercase_underscore
| Rule | Definition | Example
|--|--|--|
| `<where>_screen_<widget>_<description>` <br> or <br> `<where>_<widget>_<description>` <br> or <br>`<widget>_<description>` <br> or <br> `<attribute>_<description>` | **where** =  where it's used(activity,fragment,dialog) <br> **widget** = widget name(button, image etc) <br> **attribute** = margin, padding | ◾`<dimen name="user_detail_screen_cardview_radius">4dp</dimen>`  <br> ◾`<dimen name="dialog_icon_height">16dp</dimen>` <br> ◾`<dimen name="image_width">120dp</dimen>` <br> ◾`<dimen name="margin_medium">16dp</dimen>`|

<br>

### 🔸ID's in XML

    lowerCamelCase

| Rule | Definition | Example
|--|--|--|
| `<view><What>` | **view** = Short name of the view <br> Button - btn <br> Spinner - spn<br> EditText - et <br> TextView - tv <br> RecyclerView - rv <br> ConstraintLayout - cl <br> LinearLayout - ll  | ◾`btnLogin` <br> ◾`tvUserName` <br> ◾`clProductContainer` |

<br>

### 🔸Resources

    lowercase_underscore
| Resource | Rule | Definition | Example
|--|--|--|--|
| Icons | `ic_<what>_<description>?` | **what** = Name of the icon <br> **description** = Description (optional) | ◾`ic_arrow_right`
| Images | `img_<what>_<description>?` |  | ◾`img_profile_placeholder` |
| Custom Drawables| `custom_<what>_<description>?` |  | ◾`custom_button_round`  |
| Partial Layouts | `partial_<what>_<description>?` | Parts of other layouts that are `<include>`d | ◾`partial_stats_container` |
| Dialogs | `dialog_<what>_<description>?` | Dialog layouts | ◾`dialog_change_theme` |
| Item Views | `item_<what>_<description>?` | Item views of List Adapters| ◾`item_bank_account` |

<br>

### 🔸Strings.xml

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `<where>_screen_<description>_<type>` <br> or <br> `<where>_<description>_<type>` <br> or <br> `common_<description>`| **where** = DieticianDetailActivity + *screen* <br> **description** = Credit card type <br> **type** = Header  | ◾`<string name="dietician_detail_screen_credit_card_type_header"> Credit Card Type </string>` <br> ◾`<string name="common_loading">Loading...</string>`|

<br>

### 🔸Styles

    PascalCase

| Rule | Definition | Example
|--|--|--|
| `<Widget><Description>`<br> or <br> `<Where><Description>` | For header texts| ◾`<style name="TextHeader" parent="Widget.AppCompat.TextView">` |
|`<Widget><Description>.<Style>`| Extends all styles from TextHeader and adds new color style | ◾`<style name="TextHeader.Black">` |

<br>

### 🔸Text Sizes

    lowercase_underscore

| Rule | Definition | Example
|--|--|--|
| `text_size_<description>`  | **description** = caption, small, medium, normal, big, headline |  ◾`<dimen name="text_size_caption "> 12sp </dimen>` 

<br>
