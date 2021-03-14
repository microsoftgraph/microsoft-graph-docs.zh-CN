---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5571e46b11113385eda8621a650a6ed2dabb4405
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignedTo = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo')
    .get();

```