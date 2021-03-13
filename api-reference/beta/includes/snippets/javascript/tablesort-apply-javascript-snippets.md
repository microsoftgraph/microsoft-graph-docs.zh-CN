---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1cd60461c14ce830e86c3807d3621400c29fce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787917"
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
  method: 'method-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply')
    .version('beta')
    .post(apply);

```