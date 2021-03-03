# CKEditor 5 with all utilities plugins

### To install:

`npm i ckeditor5-custom-build-full`

### To use:

```javascript
import { CKEditor } from "@ckeditor/ckeditor5-react";
import FullEditor from "ckeditor5-custom-build-full/build/ckeditor.js";

const Editor = ({ onChange, name, value }) => {
  return (
    <CKEditor
      editor={FullEditor}
      data={value}
      onChange={(event, editor) => {
        const data = editor.getData();
        onChange({ target: { name, value: data } });
      }}
    />
  );
};
```
