---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313ba020b67170a2077cd7d8ed2601375cec7a7c8878a85893734dbe263cea84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332179"
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

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```