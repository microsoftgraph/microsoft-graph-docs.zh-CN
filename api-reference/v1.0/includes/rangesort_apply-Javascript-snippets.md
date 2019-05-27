---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f601e69eae0eb0bec735a8cc16dfdc1645398b2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  fields: [
    {
      key: 99,
      sortOn: "sortOn-value",
      ascending: true,
      color: "color-value",
      dataOption: "dataOption-value",
      icon: {
        set: "set-value",
        index: 99
      }
    }
  ],
  matchCase: true,
  hasHeaders: true,
  orientation: "orientation-value",
  method: "method-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort/apply')
    .post(apply);

```