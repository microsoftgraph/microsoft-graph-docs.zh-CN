---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f4bbe61666174dceffedc03ec3ca3b76d332fdb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478891"
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

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/add')
    .version('beta')
    .post(workbookTableRow);

```