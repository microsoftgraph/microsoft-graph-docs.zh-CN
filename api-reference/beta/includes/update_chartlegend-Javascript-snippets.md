---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c5bbf7bf64008a178af825c225240744c5132a46
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLegend = {
  visible: true,
  position: "position-value",
  overlay: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .update({workbookChartLegend : workbookChartLegend});

```