---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aaef54f8e1eaef851c6e58f243789629ead7fed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewInstanceDecisionItem = {
  decision: 'Approve',
  justification: 'I trust this person'
};

await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c')
    .version('beta')
    .update(accessReviewInstanceDecisionItem);

```