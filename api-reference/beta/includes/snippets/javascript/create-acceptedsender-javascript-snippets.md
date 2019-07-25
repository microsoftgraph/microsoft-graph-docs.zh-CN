---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc7d8c88121ee95591ea1988708d350fadb0ec34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/beta/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/acceptedSenders/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```