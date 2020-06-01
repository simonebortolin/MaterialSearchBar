# Material SearchBar Android
[![](https://jitpack.io/v/simonebortolin/MaterialSearchBar.svg)](https://jitpack.io/#simonebortolin/MaterialSearchBar)

Android 3rd party library to make a MaterialSearchBar in a easy mode.
This beautiful and easy to use library will help to add a Material Design SearchView in your project.

## Screenshots
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_1.png" alt="" width="200px"></a>
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_2.png" alt="" width="200px"></a>
<img src="https://github.com/simonebortolin/MaterialSearchBar/blob/master/image_3.png" alt="" width="200px"></a>

## Installation

Step 1. Add it in your **root** build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

Step 2. Add the dependency

```gradle
dependencies {
	implementation 'androidx.recyclerview:recyclerview:1.1.0'
	implementation 'com.github.simonebortolin:MaterialSearchBar:1.2.1'
}
```

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

### MaterialSearchBar has the following xml attributes:

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
| mt_leftTextSelectorDrawable | set left text selector drawable                                                  |
| mt_middleTextSelectorDrawable | set middle text selector drawable                                              |
| mt_rightTextSelectorDrawable | set right text selector drawable                                                |
| mt_leftTextSelectorTint | set left text selector tint color                                                    |
| mt_middleTextSelectorTint | set middle text selector tint color                                                |
| mt_rightTextSelectorTint | set right text selector tint color                                                  |
| mt_handlesTintEnabled  | should text selectors use tint color                                                  |
| mt_highlightedTextColor | set the text highlight tint color                                                    |
| mt_suggestionsAnimationSpeed | set the animation speed |

----------

### Documentation

#### `public void inflateMenu(int menuResource)`

Inflate menu for searchBar

 * **Parameters:** `menuResource` — - menu resource

#### `public void inflateMenu(int menuResource, int icon)`

Inflate menu for searchBar with custom Icon

 * **Parameters:**
   * `menuResource` — - menu resource
   * `icon` — - icon resource id

#### `public PopupMenu getMenu()`

Get popup menu

 * **Returns:** PopupMenu

#### `private void setupRoundedSearchBarEnabled()`

Capsule shaped searchbar enabled Only works on SDK V21+ due to odd behavior on lower

#### `private void setupSearchEditText()`

Setup editText coloring and drawables

#### `public void setOnSearchActionListener(OnSearchActionListener onSearchActionListener)`

Register listener for search bar callbacks.

 * **Parameters:** `onSearchActionListener` — the callback listener

#### `public void closeSearch()`

Hides search input and close arrow

#### `public void openSearch()`

Shows search input and close arrow

#### `private void animateSuggestions(int from, int to)`

Suggestion 목록을 보여줄 때, 애니메이션을 설정한다.

#### `public boolean isSuggestionsVisible()`

Check if suggestions are shown

 * **Returns:** return result

#### `public boolean isSuggestionsEnabled()`

Check if suggestions are enabled

#### `public void setSuggestionsEnabled(boolean suggestionsEnabled)`

Set suggestions enabled

#### `public void setMenuIcon(int menuIconResId)`

Set Menu Icon Drawable

 * **Parameters:** `menuIconResId` — icon resource id

#### `public void setSearchIcon(int searchIconResId)`

Set search icon drawable

 * **Parameters:** `searchIconResId` — icon resource id

#### `public void setArrowIcon(int arrowIconResId)`

Set back arrow icon drawable

 * **Parameters:** `arrowIconResId` — icon resource id

#### `public void setClearIcon(int clearIconResId)`

Set clear icon drawable

 * **Parameters:** `clearIconResId` — icon resource id

#### `public void setNavIcon(int navIconResId)`

Set the nav icon drawable

 * **Parameters:** `navIconResId` — icon resource id

#### `public void setNavIcon()`

Set the animated nav icon drawable

#### `public void setNavIconTint(int navIconTint)`

Set the tint color of the navigation icon

 * **Parameters:** `navIconTint` — nav icon color

#### `public void setMenuIconTint(int menuIconTint)`

Set the tint color of the menu icon

 * **Parameters:** `menuIconTint` — menu icon color

#### `public void setSearchIconTint(int searchIconTint)`

Set the tint color of the search/speech icon

 * **Parameters:** `searchIconTint` — search icon color

#### `public void setArrowIconTint(int arrowIconTint)`

Set the tint color of the back arrow icon

 * **Parameters:** `arrowIconTint` — arrow icon color

#### `public void setClearIconTint(int clearIconTint)`

Set the tint color of the clear icon

 * **Parameters:** `clearIconTint` — clear icon tint

#### `public void setIconRippleStyle(boolean borderlessRippleEnabled)`

Show a borderless ripple(circular) when icon is pressed Borderless only available on SDK V21+

 * **Parameters:** `borderlessRippleEnabled` — true for borderless, false for default

#### `public void setHint(CharSequence hintText)`

Sets search bar hintText

 * **Parameters:** `hintText` — hintText text

#### `public void setPlaceHolder(CharSequence placeholder)`

Set the place holder text

 * **Parameters:** `placeholder` — placeholder text

#### `public void setSpeechMode(boolean speechMode)`

sets the speechMode for the search bar. If set to true, microphone icon will display instead of the search icon. Also clicking on this icon will trigger the callback method onButtonClicked()

 * **Parameters:** `speechMode` — enable speech
 * **See also:**
   * #BUTTON_SPEECH
   * OnSearchActionListener#onButtonClicked(int)

#### `public boolean isSpeechModeEnabled()`

True if MaterialSearchBar is in speech mode

 * **Returns:** speech mode

#### `public boolean isSearchOpened()`

Check if search bar is in edit mode

 * **Returns:** true if search bar is in edit mode

#### `public void setMaxSuggestionCount(int maxSuggestionsCount)`

Specifies the maximum number of search queries stored until the activity is destroyed

 * **Parameters:** `maxSuggestionsCount` — maximum queries

#### `public void setCustomSuggestionAdapter(SuggestionsAdapter suggestionAdapter)`

Sets a custom adapter for suggestions list view.

 * **Parameters:** `suggestionAdapter` — customized adapter

#### `public List getLastSuggestions()`

Returns the last search queries. The queries are stored only for the duration of one activity session. When the activity is destroyed, the queries will be deleted. To save queries, use the method getLastSuggestions(). To recover the queries use the method setLastSuggestions().

<b color="red">List< String > will be returned if You don't use custom adapter.</b>

 * **Returns:** array with the latest search queries
 * **See also:**
   * #setLastSuggestions(List)
   * #setMaxSuggestionCount(int)

#### `public void setLastSuggestions(List suggestions)`

Sets the array of recent search queries. It is advisable to save the queries when the activity is destroyed and call this method when creating the activity.

<b color="red">Pass a List< String > if You don't use custom adapter.</b>

 * **Parameters:** `suggestions` — an array of queries
 * **See also:**
   * #getLastSuggestions()
   * #setMaxSuggestionCount(int)

#### `public void updateLastSuggestions(List suggestions)`

Changes the array of recent search queries with animation.

<b color="red">Pass a List< String > if You don't use custom adapter.</b>

 * **Parameters:** `suggestions` — an array of queries

#### `public void setSuggstionsClickListener(SuggestionsAdapter.OnItemViewClickListener listener)`

Allows you to intercept the suggestions click event

<b color="red">This method will not work with custom Suggestion Adapter</b>

 * **Parameters:** `listener` — click listener

#### `public void setTextColor(int textColor)`

Set search input text color

 * **Parameters:** `textColor` — text color

#### `public void setTextHintColor(int hintColor)`

Set text input hintText color

 * **Parameters:** `hintColor` — text hintText color

#### `public void setPlaceHolderColor(int placeholderColor)`

Set placeholder text color

 * **Parameters:** `placeholderColor` — placeholder color

#### `public void setTextHighlightColor(int highlightedTextColor)`

Set the color of the highlight when text is selected

 * **Parameters:** `highlightedTextColor` — selected text highlight color

#### `public void setNavButtonEnabled(boolean navButtonEnabled)`

Set navigation drawer menu icon enabled

 * **Parameters:** `navButtonEnabled` — icon enabled

#### `public void setUpButtonEnabled(boolean upButtonEnabled)`

Set navigation up menu enabled. Can display back icon (up navigation icon) instead of menu button {@link #setNavButtonEnabled(boolean)}.

 * **Parameters:** `upButtonEnabled` — icon enabled

#### `public void setRoundedSearchBarEnabled(boolean roundedSearchBarEnabled)`

Enable capsule shaped SearchBar (API 21+)

 * **Parameters:** `roundedSearchBarEnabled` — capsule shape enabled

#### `public void setCardViewElevation(int elevation)`

Set CardView elevation

 * **Parameters:** `elevation` — desired elevation

#### `public String getText()`

Get search text

 * **Returns:** text

#### `public void setText(String text)`

Set search text

 * **Parameters:** `text` — text

#### `public void addTextChangeListener(TextWatcher textWatcher)`

Add text watcher to searchbar's EditText

 * **Parameters:** `textWatcher` — textWatcher to add

#### `public void removeTextChangeListener(TextWatcher textWatcher)`

Remove text watcher to searchbar's EditText

 * **Parameters:** `textWatcher` — textWatcher to add

#### `private int getListHeight(boolean isSubtraction)`

For calculate the height change when item delete or add animation false is return the full height of item, true is return the height of position subtraction one

 * **Parameters:** `isSubtraction` — is subtraction enabled

#### `public interface OnSearchActionListener`

Interface definition for MaterialSearchBar callbacks.

#### `void onSearchStateChanged(boolean enabled)`

Invoked when SearchBar opened or closed

 * **Parameters:** `enabled` — state

#### `void onSearchConfirmed(CharSequence text)`

Invoked when search confirmed and "search" button is clicked on the soft keyboard

 * **Parameters:** `text` — search input

#### `void onButtonClicked(int buttonCode)`

Invoked when "speech" or "navigation" buttons clicked.

 * **Parameters:** `buttonCode` — {@link #BUTTON_NAVIGATION}, {@link #BUTTON_SPEECH} or {@link #BUTTON_BACK} will be passed


### Example

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

    Copyright (c) 2016 mancj


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
