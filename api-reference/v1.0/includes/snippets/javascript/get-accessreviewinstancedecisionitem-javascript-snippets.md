---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19fd87de1ef37cb7162724e5be61f6e13edafb5d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstanceDecisionItem = await client.api('/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4')
    .get();

```