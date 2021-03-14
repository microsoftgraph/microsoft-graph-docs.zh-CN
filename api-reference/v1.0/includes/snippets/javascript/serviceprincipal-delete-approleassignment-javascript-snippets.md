---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 274dd00bbaadbe7a15123e711fda44a32b05ccb3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/appRoleAssignments/{id}')
    .delete();

```