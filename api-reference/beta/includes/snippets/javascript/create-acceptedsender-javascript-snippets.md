---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc7d8c88121ee95591ea1988708d350fadb0ec34
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463709"
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