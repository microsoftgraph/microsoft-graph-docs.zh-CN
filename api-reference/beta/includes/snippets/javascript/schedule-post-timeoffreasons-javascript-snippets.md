---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33aa09bda9dd097cf9cd5efc24e7b78562436fd9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499539"
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