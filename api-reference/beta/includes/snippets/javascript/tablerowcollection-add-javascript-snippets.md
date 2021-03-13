---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e0709d1c9cdd322ba58fe0a4e4c6002b1964f9f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: null,
  values: [
    [1, 2, 3],
    [4, 5, 6]
  ]
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/add')
    .version('beta')
    .post(workbookTableRow);

```