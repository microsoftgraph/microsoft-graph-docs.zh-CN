---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d821a776b6f5c2d212b4bb8d3b9892edab67fcac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let recentPlans = await client.api('/me/planner/recentPlans')
    .version('beta')
    .get();

```