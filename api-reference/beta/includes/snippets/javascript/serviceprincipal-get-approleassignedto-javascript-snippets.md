---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c05ecfd8fd2043374c06f7e1c464e1bf7137bb07
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignedTo = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo')
    .version('beta')
    .get();

```