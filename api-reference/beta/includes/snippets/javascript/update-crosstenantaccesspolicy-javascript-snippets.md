---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cfb7369dd7b0d1d55ae248162353427b489b025
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694970"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const crossTenantAccessPolicy = {
  allowedCloudEndpoints: ['microsoftonline.us', 'partner.microsoftonline.cn']
};

await client.api('/policies/crossTenantAccessPolicy')
    .version('beta')
    .update(crossTenantAccessPolicy);

```