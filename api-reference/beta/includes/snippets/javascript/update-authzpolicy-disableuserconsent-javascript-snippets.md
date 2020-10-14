---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d15ae49c381f76a6fa5050847c3b2c9a3e1bf6c9
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
    permissionGrantPolicyIdsAssignedToDefaultUserRole: [ ]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```