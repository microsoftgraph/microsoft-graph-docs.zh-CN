---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2d92513321fa085f67e729554a3cce8903eebab
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
    permissionGrantPolicyIdsAssignedToDefaultUserRole: [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```