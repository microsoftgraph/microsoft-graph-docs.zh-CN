---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a40c07c0f4e7ec430f7d4c86aa09415405be9490
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserCounts(period='D7')')
    .get();

```