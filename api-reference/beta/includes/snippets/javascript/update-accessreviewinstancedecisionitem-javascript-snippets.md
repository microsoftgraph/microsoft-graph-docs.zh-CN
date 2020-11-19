---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 7ffa51b48c4b71dd2fc7e6065a026c919c7824fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewInstanceDecisionItem = {
  decision: "Approve",
  justification: "I trust this person"
};

let res = await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c')
    .version('beta')
    .update(accessReviewInstanceDecisionItem);

```