---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ca7c0eaf4ec90775f38228b0b5606c1d633adaf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/acceptedSenders/$ref')
    .post({directoryObject : directoryObject});

```