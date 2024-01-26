# web-share-api
An easy implementation of the Web Share API to display a share sheet on any page across compatible devices.
## Logic of the code:

- Title is pulled using `document.title`, which means whatever is placed between the `<title></title>` will be used.
- The description is pulled from the `<meta>` element the attribute `name="description"`.
- The URL is pulled from `document.location.href`.
## Device behaviour
### Not working?
If it seems like the code isn't working with the device you are testing on, it is important to keep in mind that devices handle the Web Share API differently.
### Windows

- Displays the website home URL and the URL of the page being shared.
- Both the title and text field seem to be ignored.
- No image is displayed.

### Android (tested with Google Pixel)

- Displays the text (description) and URL of the page being shared.
- If the text field isn't present, the title is used as a fallback.

#### Update
- Chrome on Android now displays the title, description, and URL

### MacOS
- untested

### iOS
- untested
