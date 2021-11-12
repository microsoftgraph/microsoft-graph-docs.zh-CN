---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dd9d089986b45b88cc3de611ef829129c19ddd653990b5a9cdc6260455860dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const temporaryAccessPassAuthenticationMethod = {
  '@odata.type': '#microsoft.graph.temporaryAccessPassAuthenticationMethod',
  startDateTime: '2021-01-26T00:00:00.000Z',
  lifetimeInMinutes: 60,
  isUsableOnce: false
};

await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods')
    .version('beta')
    .post(temporaryAccessPassAuthenticationMethod);

```