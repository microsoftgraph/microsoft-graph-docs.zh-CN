---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7d8e503c568a0dc0abcd52a9d73bdf7b1cc002fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')')
    .get();

```