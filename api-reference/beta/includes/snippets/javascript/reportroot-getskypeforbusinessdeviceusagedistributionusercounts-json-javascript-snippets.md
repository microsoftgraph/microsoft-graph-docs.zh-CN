---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6dc46ec8201f3f041debd7de87e221e6aa255c64
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```