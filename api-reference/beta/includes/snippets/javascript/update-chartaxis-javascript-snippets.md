---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f53b7f9bb4bb0fc9a67095155ab3ddf51d3177f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480011"
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