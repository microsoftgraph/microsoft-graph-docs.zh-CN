---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4441e1b166ed6a14e57ada029aee1a7e18cfcd5b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636500"
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
    .post(directoryObject);

```