---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 78e69d34e5770ea7cfa2ae29931a84f655258732
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt')
    .version('beta')
    .post({workbookChart : workbookChart});

```