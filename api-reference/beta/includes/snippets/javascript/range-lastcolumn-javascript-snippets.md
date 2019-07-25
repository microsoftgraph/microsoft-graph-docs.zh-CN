---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa7d9642e9463acd12a42e66837f3bd323cabe9a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728116"
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