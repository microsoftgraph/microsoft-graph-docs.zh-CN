---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d406f3b780c0f0e71341725446834f0ecbe372b6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788303"
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

await client.api('/serviceprincipals/{id}/removeKey')
    .version('beta')
    .post(removeKey);

```