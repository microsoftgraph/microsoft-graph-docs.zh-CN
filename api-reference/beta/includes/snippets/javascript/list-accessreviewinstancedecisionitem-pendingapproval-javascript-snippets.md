---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6102b40e877e28175ead3eaa5cae9e9dfd00ca7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```