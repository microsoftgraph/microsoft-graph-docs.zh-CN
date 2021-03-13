---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 131a6d517f7667f2219df1379e6cf580da36613f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  displayName: 'John Smith',
  identities: [
    {
      signInType: 'userName',
      issuer: 'contoso.onmicrosoft.com',
      issuerAssignedId: 'johnsmith'
    },
    {
      signInType: 'emailAddress',
      issuer: 'contoso.onmicrosoft.com',
      issuerAssignedId: 'jsmith@yahoo.com'
    },
    {
      signInType: 'federated',
      issuer: 'facebook.com',
      issuerAssignedId: '5eecb0cd'
    }
  ],
  passwordProfile: {
    password: 'password-value',
    forceChangePasswordNextSignIn: false
  },
  passwordPolicies: 'DisablePasswordExpiration'
};

await client.api('/users')
    .version('beta')
    .post(user);

```