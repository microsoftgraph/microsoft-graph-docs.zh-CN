---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a718a4244659280aa4b7ed8596ae6ebde95a1e58
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  grantees: [
    {
      email: "ryan@contoso.com"
    }
  ]
};

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants')
    .version('beta')
    .post(permission);

```