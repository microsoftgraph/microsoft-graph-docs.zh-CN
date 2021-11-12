---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df7a1218655445d9d35065be3de5aca2ea93285ec52e9bc4bcb1a3ac602d6c4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215643"
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

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .update(workbookChartDataLabels);

```