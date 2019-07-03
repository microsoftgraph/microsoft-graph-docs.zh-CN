---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0abb3f997dffb514c231de849b334bf44ebb9924
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .skip(5)
    .top(5)
    .get();

```