---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e4920fe88da88fabac31bd31939546275cd99289
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/groups/{id}/owners/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```