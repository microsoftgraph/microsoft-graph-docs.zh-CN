---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea19196a2358d05e7cd831df9b29921f3b229fd9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6',
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/applications/{id}/removeKey')
    .version('beta')
    .post(removeKey);

```