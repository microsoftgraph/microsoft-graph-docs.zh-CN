---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c490ee6291c46b527bc87c281e5c998714c8e45
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316515"
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
    .update(user);

```