---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33aa09bda9dd097cf9cd5efc24e7b78562436fd9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: "Vacation",
  iconType: "plane",
  isActive: true
};

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .post({timeOffReason : timeOffReason});

```