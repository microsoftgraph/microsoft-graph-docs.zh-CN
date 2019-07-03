---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b2606c6b2c437b4473da062e4dae24690d90c2a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  displayName: "displayName-value",
  mailNickname: "mailNickname-value",
  userPrincipalName: "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    forceChangePasswordNextSignIn: true,
    password: "password-value"
  }
};

let res = await client.api('/users')
    .version('beta')
    .post({user : user});

```