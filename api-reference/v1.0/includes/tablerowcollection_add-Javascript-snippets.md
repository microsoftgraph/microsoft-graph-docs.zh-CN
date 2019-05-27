---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c21351dc7a1df9b0b3cee8d335eef2fc4e9ab83
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 5,
  values: [
    [1, 2, 3],
    [4, 5, 6]
  ]
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/add')
    .post(workbookTableRow);

```