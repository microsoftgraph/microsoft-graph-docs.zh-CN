---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57fe99fd0c17a3ea48a87cd7654a2adc6a59e8a47f35e10ac578e9d36373c5ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   enabledPreviewFeatures: [
      'assignGroupsToRoles'
   ]
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```