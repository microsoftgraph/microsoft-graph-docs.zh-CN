---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a54bf18544221e3d0cc52582d4fb9281ae4359a0941c444d9d0f4eae238ddac8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333999"
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