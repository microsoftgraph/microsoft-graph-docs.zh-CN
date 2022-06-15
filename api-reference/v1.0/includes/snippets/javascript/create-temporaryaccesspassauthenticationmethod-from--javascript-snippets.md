---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db7a595dd1e83ab0b9212c95094a5a205d1a103f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093338"
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
    .post(temporaryAccessPassAuthenticationMethod);

```