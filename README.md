### Example 1: Basic Text Message with a Single Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Hello!',
  text: 'This is a basic interactive message.',
  footer: 'Footer Text',
  buttons: [
    { type: 'button', display_text: 'Click Me', id: 'btn_1' }
  ]
});
```

### Example 2: Text Message with URL Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Visit Our Website',
  text: 'Click the button below to visit our website.',
  footer: 'Footer Text',
  buttons: [
    { type: 'url', display_text: 'Visit', url: 'https://example.com' }
  ]
});
```

### Example 3: Text Message with Address Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Our Office Address',
  text: 'Click the button to view our address.',
  footer: 'Footer Text',
  buttons: [
    { type: 'address', display_text: 'View Address', id: 'address_1' }
  ]
});
```

### Example 4: Text Message with Location Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Share Your Location',
  text: 'Click the button to share your location with us.',
  footer: 'Footer Text',
  buttons: [
    { type: 'location', display_text: 'Share Location' }
  ]
});
```

### Example 5: Text Message with Copy Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Copy This Code',
  text: 'Click the button to copy the code.',
  footer: 'Footer Text',
  buttons: [
    { type: 'copy', display_text: 'Copy Code', id: 'copy_1', copy_code: 'ABC123' }
  ]
});
```

### Example 6: Text Message with Call Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Call Us',
  text: 'Click the button to call us.',
  footer: 'Footer Text',
  buttons: [
    { type: 'call', display_text: 'Call', phone_number: '+1234567890' }
  ]
});
```

### Example 7: Text Message with List of Items
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Choose an Option',
  text: 'Select an item from the list below.',
  footer: 'Footer Text',
  buttons: [
    { type: 'list', maintitle: 'Options', header: 'Header 1', title: 'Option 1', description: 'Description 1', id: 'opt_1' },
    { type: 'list', maintitle: 'Options', header: 'Header 2', title: 'Option 2', description: 'Description 2', id: 'opt_2' }
  ]
});
```

### Example 8: Text Message with Image Attachment
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Check this out!',
  text: 'Here is an image for you.',
  footer: 'Footer Text',
  image: 'path/to/image.jpg',
  buttons: [
    { type: 'button', display_text: 'Like', id: 'btn_like' }
  ]
});
```

### Example 9: Text Message with Video Attachment
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Watch this Video',
  text: 'Here is a video for you.',
  footer: 'Footer Text',
  video: 'path/to/video.mp4',
  buttons: [
    { type: 'button', display_text: 'Watch Again', id: 'btn_watch_again' }
  ]
});
```

### Example 10: Text Message with Multiple Button Types
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Multiple Actions',
  text: 'Choose an action below.',
  footer: 'Footer Text',
  buttons: [
    { type: 'button', display_text: 'Simple Button', id: 'btn_simple' },
    { type: 'url', display_text: 'Visit Site', url: 'https://example.com' },
    { type: 'call', display_text: 'Call Us', phone_number: '+1234567890' }
  ]
});
```

### Example 11: Text Message with List and Media Attachment
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Select an Option',
  text: 'Choose from the list below.',
  footer: 'Footer Text',
  image: 'path/to/image.jpg',
  buttons: [
    { type: 'list', maintitle: 'Section 1', header: 'Header 1', title: 'Item 1', description: 'Description 1', id: 'item_1' },
    { type: 'list', maintitle: 'Section 2', header: 'Header 2', title: 'Item 2', description: 'Description 2', id: 'item_2' }
  ]
});
```

### Example 12: Text Message with Call and URL Buttons
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Contact Us',
  text: 'You can call us or visit our website.',
  footer: 'Footer Text',
  buttons: [
    { type: 'call', display_text: 'Call', phone_number: '+1234567890' },
    { type: 'url', display_text: 'Visit Site', url: 'https://example.com' }
  ]
});
```

### Example 13: Text Message with Address and Copy Buttons
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Get Details',
  text: 'View our address or copy the code.',
  footer: 'Footer Text',
  buttons: [
    { type: 'address', display_text: 'View Address', id: 'address_1' },
    { type: 'copy', display_text: 'Copy Code', id: 'copy_1', copy_code: 'ABC123' }
  ]
});
```

### Example 14: Text Message with Location and Simple Button
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Actions',
  text: 'Share your location or click the button.',
  footer: 'Footer Text',
  buttons: [
    { type: 'location', display_text: 'Share Location' },
    { type: 'button', display_text: 'Click Me', id: 'btn_1' }
  ]
});
```

### Example 15: Text Message with Copy and URL Buttons
```javascript
await client.interactiveMessage(m.jid, {
  title: 'Get Code or Visit Site',
  text: 'Copy the code or visit our website.',
  footer: 'Footer Text',
  buttons: [
    { type: 'copy', display_text: 'Copy Code', id: 'copy_1', copy_code: 'ABC123' },
    { type: 'url', display_text: 'Visit Site', url: 'https://example.com' }
  ]
});
```
