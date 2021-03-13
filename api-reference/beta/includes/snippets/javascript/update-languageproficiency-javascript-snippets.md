---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c15834edea5df67fed9fa98d03c0f974e421305
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  allowedAudiences: 'organization'
};

await client.api('/me/profile/languages/{id}')
    .version('beta')
    .update(languageProficiency);

```