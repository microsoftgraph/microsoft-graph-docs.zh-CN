---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1907aa76251e46bc27db38eff9eae5570bb18b361d05670232f1ced5175a37a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions: {
      permissionGrantPoliciesAssigned: [
         'managePermissionGrantsForSelf.microsoft-user-default-low'
      ]
   }
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```