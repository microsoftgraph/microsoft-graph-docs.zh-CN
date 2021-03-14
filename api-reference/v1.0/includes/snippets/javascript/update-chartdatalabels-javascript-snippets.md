---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc7191c6ac550283a966c3db67b6f0cd0cd5d443
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartDataLabels = {
  position: 'position-value',
  showValue: true,
  showSeriesName: true,
  showCategoryName: true,
  showLegendKey: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .update(workbookChartDataLabels);

```