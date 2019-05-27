---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c4ca1d45fde32bb8c16cf77407fb2f0294db4fd7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456121"
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
    .version('beta')
    .post(workbookChart);

```