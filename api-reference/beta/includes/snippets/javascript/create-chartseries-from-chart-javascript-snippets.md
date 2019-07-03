---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b6c821b69aa6dddf165ea7691932ecd93e9a2fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .version('beta')
    .post({workbookChartSeries : workbookChartSeries});

```