---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 18163aa07fa813d89e642b7a68b10b4c56fe46d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500597"
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