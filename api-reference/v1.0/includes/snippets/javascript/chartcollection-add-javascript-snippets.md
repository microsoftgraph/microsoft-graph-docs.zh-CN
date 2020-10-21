---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf34385fc458c019a243b672a38f66c47e1bae96
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  type: "ColumnStacked",
  sourceData: "A1:B1",
  seriesBy: "Auto"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add')
    .post(workbookChart);

```