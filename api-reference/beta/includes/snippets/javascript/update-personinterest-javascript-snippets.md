---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb9b7d48cd5fa74bbc633df4a88acfc9994c866
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    'Sports'
  ]
};

await client.api('/me/profile/interests/{id}')
    .version('beta')
    .update(personInterest);

```