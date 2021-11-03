---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a911ce6eafa70ee8ffafa4c1c90aa2132695620
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: 'everyone',
      value: '67a141d8-cf4e-4528-ba07-bed21bfacd2d',
      accessType: 'grant',
      identitySource: 'azureActiveDirectory'
    }
  ]
};

await client.api('/external/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```