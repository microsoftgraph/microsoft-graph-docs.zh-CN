---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f73563eb9aef9e162f437d3c94a0701752e8f28f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```