---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c27351c3d2a4e6c8d70d0f00c15b12c30be5b22bfdfdf42366ae1f608b3c80ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  passwordProfile: {
    forceChangePasswordNextSignIn: false,
    password: 'xWwvJ]6NMw+bWH-d'
  }
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```