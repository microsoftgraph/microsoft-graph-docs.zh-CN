---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d48fb3ab36880d376ed338612eb1867397c7b525e127a9480ddbc57a7d92e1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161323"
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