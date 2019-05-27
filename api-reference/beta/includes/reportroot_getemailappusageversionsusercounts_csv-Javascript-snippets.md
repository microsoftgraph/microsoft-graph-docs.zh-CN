---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 466218397e6490804ec2a32f7409f5143f7f0e90
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageVersionsUserCounts(period='D7')')
    .version('beta')
    .get();

```