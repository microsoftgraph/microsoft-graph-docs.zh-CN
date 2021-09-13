---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9eff980c854bb5ae1a45aedcbbe8738a7c3e9184afa64641eab2d1a5649c4bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstanceDecisionItem = await client.api('/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4')
    .get();

```