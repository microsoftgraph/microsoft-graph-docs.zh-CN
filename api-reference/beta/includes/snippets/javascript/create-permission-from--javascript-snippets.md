---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b83d5451ee4a8620e0904465d506b754cf48b70
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ["write"],
  grantedToIdentities: [{
    application: {
      id: "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      displayName: "Foo App"
    }
  }]
};

let res = await client.api('/sites/{sitesId}/permissions')
    .version('beta')
    .post(permission);

```