---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa7d9642e9463acd12a42e66837f3bd323cabe9a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastColumn')
    .version('beta')
    .get();

```