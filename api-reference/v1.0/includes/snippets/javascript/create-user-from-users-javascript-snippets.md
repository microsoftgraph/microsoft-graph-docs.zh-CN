---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3165c1784d6892e6ab4a60df1eee96737aed9e52
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711371"
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
    .post({user : user});

```