---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a89a082d852cf2d4bdca68273a4f77f953b42d18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')')
    .get();

```