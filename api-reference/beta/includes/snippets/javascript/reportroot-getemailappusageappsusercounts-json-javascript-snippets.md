---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1a2b65c182ae0ef09898e64518e3496e69c6e79
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageAppsUserCounts(period='D7')')
    .version('beta')
    .get();

```