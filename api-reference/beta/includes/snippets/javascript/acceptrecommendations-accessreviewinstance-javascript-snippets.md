---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 120aac617a9277e3d4e713a3999aaf1a372da14e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781652"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations')
    .version('beta')
    .post();

```