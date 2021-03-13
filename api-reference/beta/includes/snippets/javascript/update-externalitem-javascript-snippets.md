---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a7cc915fe05de0169005410cd2971d4c0003cbf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796927"
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

await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```