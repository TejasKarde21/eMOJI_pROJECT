# eMOJI_pROJECT

Display Submit Button: Inside searchEmoji, there is a conditional check to determine if the value of the searchField input is not empty (searchField.value !== ""). If it's not empty, it sets the CSS display property of the submitButton to "flex" to make it visible. If it's empty, it hides the submitButton by setting its display property to "none."

*Logging Submit Button: It logs the submitButton to the console to track its visibility status.
*Function Invocation Log: Logs "function called" to the console. This log helps track when the searchEmoji function is invoked.
*Get Input Value: Retrieves the current value of the searchField input element and assigns it to the searchFieldValue variable.

*Filter Emoji List: It filters an array called emojiList based on the searchFieldValue. It checks if any of the elements in emojiList have aliases or tags that start with searchFieldValue. If a match is found, the element is included in the filteredList.

*Clearing Search Result Container: Clears the content of an HTML element with the ID "searchResultContainer" to prepare it for displaying the filtered results.

*Generating Results: It iterates through the filteredList and, for each element, creates three HTML elements: an h1 for the emoji, a p for the description, and an h3 for the category. It sets the text content of these elements to the corresponding properties of the ele object in the filtered list.

*Appending Results: It appends these newly created elements (emoji, category, and description) as children to the "searchResultContainer" element, effectively displaying the filtered emoji results.

*Initial Submit Button State: There's an initial check to see if the searchField is empty (searchField.value == ""). If it is, the submitButton is initially set to be hidden (display: none).

*Event Listeners: Two event listeners are set up:

*When the "submitButton" is clicked, the searchEmoji function is called.
When a key is released (keyup) in the searchField, the searchEmoji function is called, allowing for real-time search updates as the user types.
On Page Load: The searchEmoji function is called when the page loads (window.onload). This ensures that any initial emoji data matching the empty search field is displayed when the page is first loaded.
