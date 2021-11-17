---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c84cef28a70fa21d077588cd6a64c8b014c7e691a6a121c5c47575c301f9a35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions: {
      allowedToCreateApps: false
   }
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```