---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 047f400c76f70666b44355abf20356dee758d4f1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartDataLabels = {
  position: "position-value",
  showValue: true,
  showSeriesName: true,
  showCategoryName: true,
  showLegendKey: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .update({workbookChartDataLabels : workbookChartDataLabels});

```