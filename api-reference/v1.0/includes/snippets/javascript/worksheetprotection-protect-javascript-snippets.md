---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e829f0bfba35226b0441f72bb20ed98f456fe1c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const protect = {
  options: {
    allowFormatCells: true,
    allowFormatColumns: true,
    allowFormatRows: true,
    allowInsertColumns: true,
    allowInsertRows: true,
    allowInsertHyperlinks: true,
    allowDeleteColumns: true,
    allowDeleteRows: true,
    allowSort: true,
    allowAutoFilter: true,
    allowPivotTables: true
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect')
    .post(protect);

```