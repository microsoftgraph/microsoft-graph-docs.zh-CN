---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12e937d4931a8f7217bec201dbc5e6a087d85653
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/beta/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```