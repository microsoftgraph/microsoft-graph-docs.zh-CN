---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e829f0bfba35226b0441f72bb20ed98f456fe1c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493369"
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