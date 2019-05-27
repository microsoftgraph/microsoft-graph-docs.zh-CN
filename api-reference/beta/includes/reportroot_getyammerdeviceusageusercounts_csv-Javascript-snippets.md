---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bef00660b19542d04996732bc59e4a5b5badcf2f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```