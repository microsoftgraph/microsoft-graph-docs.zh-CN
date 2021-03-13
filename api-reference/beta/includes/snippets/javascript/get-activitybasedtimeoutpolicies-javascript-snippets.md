---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92f34713581633682e99927da63fd343e8a12201
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicies = await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .get();

```