---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d0a5095f8a5f5231e9b68a7dc7b2a2c54ce3d86d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479128"
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