---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c820fdfdbf5be4d8b7cc4bd6c45638f158aa4781
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt')
    .post({workbookChartPoint : workbookChartPoint});

```