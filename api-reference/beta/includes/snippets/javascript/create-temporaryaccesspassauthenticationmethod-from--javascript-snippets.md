---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b830e8b09f3c13eaf88e4c44115d5bef791e10a5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const temporaryAccessPassAuthenticationMethod = {
    startDateTime: '2022-06-05T00:00:00.000Z',
    lifetimeInMinutes: 60,
    isUsableOnce: false
};

await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods')
    .version('beta')
    .post(temporaryAccessPassAuthenticationMethod);

```