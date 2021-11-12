---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66a325051a9fe3564f876be55bd5308c1511b23456f1d31364d03436f7fa54c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewInstanceDecisionItem = {
  decision: 'Approve',
  justification: 'This person is still on my team',
};

await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19')
    .version('beta')
    .update(accessReviewInstanceDecisionItem);

```