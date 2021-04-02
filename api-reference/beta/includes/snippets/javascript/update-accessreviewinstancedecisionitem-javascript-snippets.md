---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7a7115bb19c1eb2491e4b898f9cf3b973471943
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507218"
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