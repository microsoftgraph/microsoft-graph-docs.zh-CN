---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa2e4ae6b499f00db1611e42faa7c1cbef1e0d90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRoster = {
  '@odata.type': '#microsoft.graph.plannerRoster'
};

await client.api('/planner/rosters')
    .version('beta')
    .post(plannerRoster);

```