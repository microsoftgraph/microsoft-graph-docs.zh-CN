---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6d52b617c748c2fed67c441d325c5015a1372b5f7b2ad4af2fe1cd9268babda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewInstanceDecisionItem = {
  decision: 'Approve',
  justification: 'Kathleen still needs access to the Marketing group as she works in the Marketing organization.'
};

await client.api('/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555')
    .update(accessReviewInstanceDecisionItem);

```