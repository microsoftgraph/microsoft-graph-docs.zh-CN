---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c94ada8111a7e74c9031cc524d2776bcf2ef96f
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  displayName: "John Smith",
  identities: [
    {
      signInType: "signInName",
      issuer: "contoso.onmicrosoft.com",
      issuerAssignedId: "johnsmith"
    },
    {
      signInType: "federated",
      issuer: "facebook.com",
      issuerAssignedId: "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    forceChangePasswordNextSignIn: true,
    password: "password-value"
  }
};

let res = await client.api('/users')
    .version('beta')
    .post(user);

```