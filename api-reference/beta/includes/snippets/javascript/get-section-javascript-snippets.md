---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0fb2a4ea83b84b1f5331288f3b985d5bb6ffaccd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections/{id}')
    .version('beta')
    .get();

```