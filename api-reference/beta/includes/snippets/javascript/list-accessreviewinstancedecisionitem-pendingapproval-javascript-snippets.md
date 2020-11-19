---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: aa06dadd2653c382337b3a17cebcd015049806d5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```