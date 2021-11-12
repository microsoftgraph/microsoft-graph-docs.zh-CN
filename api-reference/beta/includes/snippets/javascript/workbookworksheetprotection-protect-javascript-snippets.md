---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb5a32993adfaa8c279d925f244b4aad8e14320c920480232c85fd5efb9e21b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218436"
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

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect')
    .version('beta')
    .post(protect);

```