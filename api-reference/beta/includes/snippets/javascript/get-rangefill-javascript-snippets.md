---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0fbdd8c0041e4e76f1af16b22e8ca35e2ab05e3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .get();

```