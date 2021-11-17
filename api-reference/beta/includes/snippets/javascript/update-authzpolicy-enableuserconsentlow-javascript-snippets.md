---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b0dfbae713670830372220639ea8f7462414c7fcafd274d57f151ffe3f7c7b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   permissionGrantPolicyIdsAssignedToDefaultUserRole: [
      'managePermissionGrantsForSelf.microsoft-user-default-low'
   ]
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```