# Material SearchBar Android
[![](https://jitpack.io/v/simonebortolin/MaterialSearchBar.svg)](https://jitpack.io/#simonebortolin/MaterialSearchBar)

<<<<<<< HEAD
Android 3rd party library to make a MaterialSearchBar in a easy mode. 
This beautiful and easy to use library will help to add a Material Design SearchView in your project.
=======
# Material SearchBar Android
Material Design Search Bar for Android
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-MaterialSearchBar-orange.svg?style=flat)](http://android-arsenal.com/details/1/4158)
[![](https://jitpack.io/v/mancj/MaterialSearchBar.svg)](https://jitpack.io/#mancj/MaterialSearchBar)

----------
This beautiful and easy to use library will help to add Lollipop Material Design SearchView in your project.

<img src="/art/preview.gif" width="400">
<img src="/art/pv1.png" width="400">
<img src="/art/pv2.png" width="400">
<img src="/art/pv3.png" width="400">
<img src="/art/pv4.png" width="400">
<img src="/art/pv5.png" width="400">

----------
>>>>>>> ae97157dfe6d0219bdbc1f9ad06e88274a7ca326

## Screenshots
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_1.png" alt="" width="200px"></a>
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_2.png" alt="" width="200px"></a>
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_3.png" alt="" width="200px"></a>

## Installation

<<<<<<< HEAD
Step 1. Add it in your **root** build.gradle at the end of repositories:
=======
# How to use
>>>>>>> ae97157dfe6d0219bdbc1f9ad06e88274a7ca326

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

Step 2. Add the dependency

```gradle
dependencies {
<<<<<<< HEAD
	implementation 'com.github.simonebortolin:MaterialSearchBar:0.10'
=======
	implementation 'com.github.mancj:MaterialSearchBar:X.X.X'
>>>>>>> ae97157dfe6d0219bdbc1f9ad06e88274a7ca326
}
```
[![](https://jitpack.io/v/mancj/MaterialSearchBar.svg)](https://jitpack.io/#mancj/MaterialSearchBar)

## How to use this library

then add SearchBar to your activity:

```xml
<com.mancj.materialsearchbar.MaterialSearchBar
    style="@style/MaterialSearchBarLight"
    app:mt_speechMode="true"
    app:mt_hint="Custom hint"
    app:mt_maxSuggestionsCount="10"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:id="@+id/searchBar" />
```

----------

**MaterialSearchBar has the following xml attributes:**

| Attribute              | Description                                                                           |
|------------------------|---------------------------------------------------------------------------------------|
| mt_speechMode          | if set to true, microphone icon will be displayed instead of search icon    	 	     |
| mt_maxSuggestionsCount | specifies the max number of search queries stored                                     |
| mt_navIconEnabled      | set navigation icon enabled                                                           |
| mt_roundedSearchBarEnabled | use capsule shaped searchbar on v21+ and revert to default on lower               |
| mt_dividerColor        | set the colors of the suggestion and menu dividers   				                 |
| mt_searchBarColor      | set the main color of the searchbar                                                   |
| mt_menuIconDrawable    | set drawable of the menu icon                                                         |
| mt_searchIconDrawable  | set drawable of the search icon when speech mode is false                             |
| mt_speechIconDrawable  | set drawable of the speech icon when speech mode is true                              |
| mt_backIconDrawable    | set drawable of the back arrow icon                                                   |
| mt_clearIconDrawable   | set drawable of the clear icon                                                        |
| mt_navIconDrawable     | set drawable of the nav icon                                                          |
| mt_navIconTint         | set tint color of nav/back animated icon                                              |
| mt_menuIconTint        | set tint color of the menu icon                                                       |
| mt_searchIconTint      | set tint color search/speech icon                                                     |
| mt_backIconTint        | set tint color of the back arrow icon                                                 |
| mt_clearIconTint       | set tint color of the clear icon                                                      |
| mt_navIconUseTint      | should the animated nav icon use tint color                                           |
| mt_menuIconUseTint     | should the menu icon use the tint color                                               |
| mt_searchIconUseTint   | should the search/speech icon use the tint color                                      |
| mt_backIconUseTint     | should the back icon use the tint color                                               |
| mt_clearIconUseTint    | should the clear icon use the tint color                                              |
| mt_hint                | set the text of the hint when the searchbar is focused and search query is empty      |
| mt_placeholder         | set the placeholder text when the MaterialSearchBar is not focused                    |
| mt_textColor           | set text color                                                                        |
| mt_hintColor           | set hint color                                                                        | 
| mt_placeholderColor    | set placeholder color                                                                 |
| mt_textCursorTint      | set text cursors tint                                                                 |
| mt_highlightedTextColor | set the text highlight tint color                                                    |

----------
**public methods:**

 - `addTextChangeListener(TextWatcher textWatcher)`
 - `clearSuggestions()`
 - `closeSearch()`
 - `openSearch()`
 - `getLastSuggestions()`
 - `getMenu()`
 - `getText()`
 - `hideSuggestionList()`
 - `inflateMenu(int menuResource)`
 - `inflateMenu(int menuResource, int icon)`
 - `isSearchOpened()`
 - `isSpeechModeEnabled()`
 - `isSuggestionsVisible()`
 - `setArrowIcon(int arrowIconResId)`
 - `setArrowIconTint(int arrowIconTint)`
 - `setCardViewElevation(int elevation)`
 - `setClearIcon(int clearIconResId)`
 - `setClearIconTint(int clearIconTint)`
 - `setCustomSuggestionAdapter(SuggestionsAdapter suggestionAdapter)`
 - `setDividerColor(int dividerColor)`
 - `setHint(CharSequence hintText)`
 - `setIconRippleStyle(boolean borderlessRippleEnabled)`
 - `setLastSuggestions(List suggestions)`
 - `setMaxSuggestionCount(int maxSuggestionsCount)`
 - `setMenuDividerEnabled(boolean menuDividerEnabled)`
 - `setMenuIcon(int menuIconResId)`
 - `setNavIcon(int navIconResId)`
 - `setNavIcon()`
 - `setMenuIconTint(int menuIconTint)`
 - `setNavButtonEnabled(boolean navButtonEnabled)`
 - `setNavIconTint(int navIconTint)`
 - `setOnSearchActionListener(OnSearchActionListener onSearchActionListener)`
 - `setPlaceHolder(CharSequence placeholder)`
 - `setPlaceHolderColor(int placeholderColor)`
 - `setRoundedSearchBarEnabled(boolean roundedSearchBarEnabled)`
 - `setSearchIcon(int searchIconResId)`
 - `setSearchIconTint(int searchIconTint)`
 - `setSpeechModeEnabled(boolean speechMode)`
 - `setSuggestionsClickListener(SuggestionsAdapter.OnItemViewClickListener listener)`
 - `setText(String text)`
 - `setTextColor(int textColor)`
 - `setTextHighlightColor(int highlightedTextColor)`
 - `setTextHintColor(int hintColor)`
 - `showSuggestions()`
 - `updateLastSuggestions(List suggestions)`

----------

<<<<<<< HEAD
To save search queries when the activity is destroyed, use the method `searchBar.getLastSuggestions()` and then, to restore them use `searchBar.setLastSuggestions(List<String>);` as shown in the example below

### Example
=======
```xml
Provided Styles are: MaterialSearchBarLight and MaterialSearchBarDark

Example:
<style name="MyCustomTheme" parent="MaterialSearchBarLight">
     <item name="mt_searchBarColor">@color/searchBarPrimaryColor</item>
            <item name="mt_dividerColor">@color/searchBarDividerColor</item>
            <item name="mt_navIconTint">@color/searchBarNavIconTintColor</item>
            <item name="mt_searchIconTint">@color/searchBarSearchIconTintColor</item>
            <item name="mt_clearIconTint">@color/searchBarClearIconTintColor</item>
            <item name="mt_menuIconTint">@color/searchBarMenuIconTintColor</item>
            <item name="mt_backIconTint">@color/searchBarBackIconTintColor</item>
            <item name="mt_textCursorTint">@color/searchBarCursorColor</item>
            <item name="mt_textColor">@color/searchBarTextColor</item>
            <item name="mt_hintColor">@color/searchBarHintColor</item>
            <item name="mt_placeholderColor">@color/searchBarPlaceholderColor</item>
            <item name="mt_highlightedTextColor">@color/searchBarTextHighlightColor</item>
</style>
```
**OR**

**Custom Colors - colors.xml** 
Simply set/change these colors(or some) and you have your custom style.
```xml
    //Material SearchBar Light Theme Colors
        <color name="searchBarIconColor">#3a3a3a</color>
        //Base
        <color name="searchBarPrimaryColor">#FFFFFF</color>
        <color name="searchBarCursorColor">#8000a1ff</color>
        <color name="searchBarDividerColor">#1F000000</color>
    
        //Icons
        <color name="searchBarNavIconTintColor">@color/searchBarIconColor</color>
        <color name="searchBarMenuIconTintColor">@color/searchBarIconColor</color>
        <color name="searchBarSearchIconTintColor">@color/searchBarIconColor</color>
        <color name="searchBarClearIconTintColor">@color/searchBarIconColor</color>
        <color name="searchBarBackIconTintColor">@color/searchBarIconColor</color>
    
        //Text
        <color name="searchBarTextColor">#DE000000</color>
        <color name="searchBarHintColor">#42000000</color>
        <color name="searchBarPlaceholderColor">#8A000000</color>
        <color name="searchBarTextHighlightColor">#8000a1ff</color>
    
        //Base
        <color name="searchBarPrimaryColorDark">#303030</color>
        <color name="searchBarDividerColorDark">#1FFFFFFF</color>
    
        //Material SearchBar Dark Theme Colors
        <color name="searchBarIconColorDark">#00a1ff</color>
        //Icons
        <color name="searchBarNavIconTintColorDark">@color/searchBarIconColorDark</color>
        <color name="searchBarMenuIconTintColorDark">@color/searchBarIconColorDark</color>
        <color name="searchBarSearchIconTintColorDark">@color/searchBarIconColorDark</color>
        <color name="searchBarClearIconTintColorDark">@color/searchBarIconColorDark</color>
        <color name="searchBarBackIconTintColorDark">@color/searchBarIconColorDark</color>
    
        //Text
        <color name="searchBarTextColorDark">#DEFFFFFF</color>
        <color name="searchBarHintColorDark">#42FFFFFF</color>
        <color name="searchBarPlaceholderColorDark">#8AFFFFFF</color>
        <color name="searchBarTextHighlightColorDark">#BF00a1ff</color>
```
----------
To save search queries when the activity is destroyed, use the method `searchBar.getLastSuggestions()` and then, to restore them use `searchBar.setLastSuggestions(List<String>);` as shown in the example below

# Example
>>>>>>> ae97157dfe6d0219bdbc1f9ad06e88274a7ca326

Here is a simple example of using MaterialSearchBar
Kotlin

    searchBar.inflateMenu(R.menu.main)
    searchBar.text = "Hello World!"
    searchBar.setCardViewElevation(10)
    searchBar.setUpButtonEnabled(false)
    searchBar.addTextChangeListener(object : TextWatcher {
        override fun beforeTextChanged(charSequence: CharSequence, i: Int, i1: Int, i2: Int) {}

        override fun onTextChanged(charSequence: CharSequence, i: Int, i1: Int, i2: Int) {}

        override fun afterTextChanged(editable: Editable) {

        }

    })
    searchBar.setOnSearchActionListener(object : MaterialSearchBar.OnSearchActionListener {
        override fun onSearchStateChanged(enabled: Boolean) {

        }

        override fun onSearchConfirmed(text: CharSequence) {

        }

        override fun onButtonClicked(buttonCode: Int) {
            when (buttonCode) {
                MaterialSearchBar.BUTTON_NAVIGATION -> {
                }
                MaterialSearchBar.BUTTON_SPEECH -> {
                }
                MaterialSearchBar.BUTTON_BACK -> searchBar.disableSearch()
            }
        }
    })

Java


    searchBar = findViewById(R.id.searchBar);
    searchBar.inflateMenu(R.menu.main);
    searchBar.setText("Hello World!");
    searchBar.setCardViewElevation(10);
    searchBar.setUpButtonEnabled(false);
    searchBar.addTextChangeListener(new TextWatcher() {
        @Override
        public void beforeTextChanged(CharSequence charSequence, int i, int i1, int i2) {
        }

        @Override
        public void onTextChanged(CharSequence charSequence, int i, int i1, int i2) {
        }

        @Override
        public void afterTextChanged(Editable editable) {

        }

    });
    searchBar.setOnSearchActionListener(new MaterialSearchBar.OnSearchActionListener() {
        @Override
        public void onSearchStateChanged(boolean enabled) {

        }

        @Override
        public void onSearchConfirmed(CharSequence text) {

        }

        @Override
        public void onButtonClicked(int buttonCode) {
            switch (buttonCode) {
                case MaterialSearchBar.BUTTON_NAVIGATION:
                    break;
                case MaterialSearchBar.BUTTON_SPEECH:
                    break;
                case MaterialSearchBar.BUTTON_BACK:
                    searchBar.disableSearch();
                    break;
            }
        }
    });
        
However, the library is very customizable, and you can easily change the view of the adapter.


## Credits


I thank all the authors of the various commits that I have included in my fork


## License


    The MIT License (MIT)

    Copyright (c) 2016

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.

    Please let me know if you use the library in your applications.
    I want to collect and publish this list.
