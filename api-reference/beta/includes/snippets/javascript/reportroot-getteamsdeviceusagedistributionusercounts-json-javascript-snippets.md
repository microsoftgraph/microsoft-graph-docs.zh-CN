---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4422cdaa8c09156f435ad13db6bdbea98c1d9241
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```