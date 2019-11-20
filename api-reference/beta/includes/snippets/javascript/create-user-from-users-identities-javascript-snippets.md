---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 592da1e75bb04cc7378663b3a670928518d03085
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38751770"
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
      signInType: "userName",
      issuer: "contoso.onmicrosoft.com",
      issuerAssignedId: "johnsmith"
    },
    {
      signInType: "emailAddress",
      issuer: "contoso.onmicrosoft.com",
      issuerAssignedId: "jsmith@yahoo.com"
    },
    {
      signInType: "federated",
      issuer: "facebook.com",
      issuerAssignedId: "5eecb0cd"
    }
  ],
  "passwordProfile" : {
    password: "password-value"
  },
  passwordPolicies: "DisablePasswordExpiration"
};

let res = await client.api('/users')
    .version('beta')
    .post(user);

```