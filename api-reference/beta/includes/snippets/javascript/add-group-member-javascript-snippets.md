---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76b4e90ad85bd694ad22c0096a0595be7fe1b3cd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/groups/{id}/members/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```