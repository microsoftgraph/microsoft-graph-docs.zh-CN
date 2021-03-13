---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b599ab217e3cf2cfbcb12a84277d6f3faf4cda82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPatent = {
  number: 'USPTO-3954432633',
  webUrl: 'https://patents.gov/3954432633'
};

await client.api('/users/{userId}/profile/patents/{id}')
    .version('beta')
    .update(itemPatent);

```