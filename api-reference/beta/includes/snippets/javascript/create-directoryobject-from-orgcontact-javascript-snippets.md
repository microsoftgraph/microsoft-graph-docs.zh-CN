---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 443cc2319e01fdeb46fc321d6bd2eb6068d42ebc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post({directoryObject : directoryObject});

```