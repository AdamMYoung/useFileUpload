# useFileUpload
React hook for uploading files to the client.

## Usage
The hook returns a function which when called, will open the file selector. The callback provided to the function will return the selected files.

```tsx
const onUpload = useFileUpload((files) => {
        console.log(files);
    });
```

The hook also takes optional parameters to filter the file types and multiple file selection.

```tsx
const uploadOptions = { fileTypes: ['.jpg', '.png'], multiple: true };

const onUpload = useFileUpload((files) => {
        console.log(files);
}, uploadOptions);
```
