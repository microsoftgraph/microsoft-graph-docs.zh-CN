---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f53b7f9bb4bb0fc9a67095155ab3ddf51d3177f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxis = {
  majorUnit: {
  },
  maximum: {
  },
  minimum: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis')
    .version('beta')
    .update({workbookChartAxis : workbookChartAxis});

```