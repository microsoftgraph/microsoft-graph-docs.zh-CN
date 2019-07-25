---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c48a2ea5644fb5d8f04e1f79ebea03204e62b8d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```