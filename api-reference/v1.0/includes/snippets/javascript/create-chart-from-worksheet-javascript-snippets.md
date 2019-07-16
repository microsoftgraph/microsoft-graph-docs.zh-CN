---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9fc29c08ab50ddcbbed511b4f2615ec7b2533d3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  id: "id-value",
  height: 99,
  left: 99
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .post({workbookChart : workbookChart});

```