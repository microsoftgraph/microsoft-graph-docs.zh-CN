---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7db0bd14381a7051f231036671c4b383b2808ce6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appRoleAssignmentRequired: true
};

await client.api('/servicePrincipals/{id}')
    .version('beta')
    .update(servicePrincipal);

```