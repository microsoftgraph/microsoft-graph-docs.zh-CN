---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa0e5040351e62fc55892357162ec2325d4d8129
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6",
    proof:"eyJ0eXAiOiJ..."
};

let res = await client.api('/servicePrincipals/{id}/removeKey')
    .post(removeKey);

```