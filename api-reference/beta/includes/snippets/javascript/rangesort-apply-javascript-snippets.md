---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee1f56e7ae48bfb0ce01f407f443141bdac755ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801083"
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
      sortOn: 'sortOn-value',
      ascending: true,
      color: 'color-value',
      dataOption: 'dataOption-value',
      icon: {
        set: 'set-value',
        index: 99
      }
    }
  ],
  matchCase: true,
  hasHeaders: true,
  orientation: 'orientation-value',
  method: 'method-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort/apply')
    .version('beta')
    .post(apply);

```