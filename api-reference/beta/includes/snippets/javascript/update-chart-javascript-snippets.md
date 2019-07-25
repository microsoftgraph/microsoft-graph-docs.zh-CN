---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d0a5095f8a5f5231e9b68a7dc7b2a2c54ce3d86d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  height: 99,
  left: 99
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .version('beta')
    .update({workbookChart : workbookChart});

```