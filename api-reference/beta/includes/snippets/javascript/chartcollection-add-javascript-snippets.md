---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2aa1714f8dc74c1262d7b447c5793456857588ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  type: 'ColumnStacked',
  sourceData: 'A1:B1',
  seriesBy: 'Auto'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add')
    .version('beta')
    .post(workbookChart);

```