---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d026ed42263ce70e1e5c16beefb17f3e4ab501c7
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  displayName: "Adele Vance",
  mailNickname: "AdeleV",
  userPrincipalName: "AdeleV@contoso.onmicrosoft.com",
  "passwordProfile" : {
    forceChangePasswordNextSignIn: true,
    password: "xWwvJ]6NMw+bWH-d"
  }
};

let res = await client.api('/users')
    .version('beta')
    .post(user);

```