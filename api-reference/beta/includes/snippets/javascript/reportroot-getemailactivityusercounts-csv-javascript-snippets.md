---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 809173ab178f0fcd0697117fa989339300954f0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```