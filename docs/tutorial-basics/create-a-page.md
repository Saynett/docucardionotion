---
sidebar_position: 1
---

# Create a Page

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="apple" label="Apple" default>
    This is an apple 🍎
  </TabItem>
  <TabItem value="orange" label="Orange">
    This is an orange 🍊
  </TabItem>
  <TabItem value="banana" label="Banana">
    This is a banana 🍌
  </TabItem>
</Tabs>

<Tabs>
  <TabItem value="varon" label="Varón" default>
    <table>
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Valor normal</th>
          <th>Ligero</th>
          <th>Moderado</th>
          <th>Severo</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Diámetro diastólico</td>
          <td>42-58 mm</td>
          <td>59-63 mm</td>
          <td>64-68 mm</td>
          <td>>68 mm</td>
        </tr>
        <tr>
          <td>Diámetro diastólico indexado</td>
          <td>22-30 mm/m2</td>
          <td>31-33 mm/m2</td>
          <td>34-36 mm/m2</td>
          <td>>36 mm/m2</td>
        </tr>
        <tr>
          <td>Diámetro sistólico</td>
          <td>22-40 mm</td>
          <td>41-43 mm</td>
          <td>44-45 mm</td>
          <td>>45 mm</td>
        </tr>
        <tr>
          <td>Diámetro sistólico indexado</td>
          <td>13-21 mm/m2</td>
          <td>22-23 mm/m2</td>
          <td>24-25 mm/m2</td>
          <td>>25 mm/m2</td>
        </tr>
      </tbody>
    </table>
  </TabItem>
  <TabItem value="mujer" label="Mujer">
    <table>
      <thead>
        <tr>
          <th>Nombre</th>
          <th>Valor normal</th>
          <th>Ligero</th>
          <th>Moderado</th>
          <th>Severo</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Diámetro diastólico</td>
          <td>38-52 mm</td>
          <td>53-56 mm</td>
          <td>57-61 mm</td>
          <td>>61 mm</td>
        </tr>
        <tr>
          <td>Diámetro diastólico indexado</td>
          <td>23-31 mm/m2</td>
          <td>32-34 mm/m2</td>
          <td>35-37 mm/m2</td>
          <td>>37 mm/m2</td>
        </tr>
        <tr>
          <td>Diámetro sistólico</td>
          <td>22-35 mm</td>
          <td>36-38 mm</td>
          <td>39-41 mm</td>
          <td>>41 mm</td>
        </tr>
        <tr>
          <td>Diámetro sistólico indexado</td>
          <td>13-21 mm/m2</td>
          <td>22-23 mm/m2</td>
          <td>24-26 mm/m2</td>
          <td>>26 mm/m2</td>
        </tr>
      </tbody>
    </table>
  </TabItem>
</Tabs>

Add **Markdown or React** files to `src/pages` to create a **standalone page**:

- `src/pages/index.js` → `localhost:3000/`
- `src/pages/foo.md` → `localhost:3000/foo`
- `src/pages/foo/bar.js` → `localhost:3000/foo/bar`

## Create your first React Page

Create a file at `src/pages/my-react-page.js`:

```jsx title="src/pages/my-react-page.js"
import React from 'react';
import Layout from '@theme/Layout';

export default function MyReactPage() {
  return (
    <Layout>
      <h1>My React page</h1>
      <p>This is a React page</p>
    </Layout>
  );
}
```

A new page is now available at [http://localhost:3000/my-react-page](http://localhost:3000/my-react-page).

## Create your first Markdown Page

Create a file at `src/pages/my-markdown-page.md`:

```mdx title="src/pages/my-markdown-page.md"
# My Markdown page

This is a Markdown page
```

A new page is now available at [http://localhost:3000/my-markdown-page](http://localhost:3000/my-markdown-page).
