---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d557cf7427e815738bdcaab9a7d00ce3642dfc09
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080829"
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
    password: "password-value",
    forceChangePasswordNextSignIn: false
  },
  passwordPolicies: "DisablePasswordExpiration"
};

let res = await client.api('/users')
    .version('beta')
    .post(user);

```