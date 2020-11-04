---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0400a0f26a0831ce5b06c45ba661ef6710d38b3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users?filter=signInActivity/lastSignInDateTime%20le%202019-06-01T00:00:00Z')
    .filter('signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z')
    .get();

```