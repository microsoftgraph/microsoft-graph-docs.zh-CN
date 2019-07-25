---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18163aa07fa813d89e642b7a68b10b4c56fe46d0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/recentPlans')
    .version('beta')
    .get();

```