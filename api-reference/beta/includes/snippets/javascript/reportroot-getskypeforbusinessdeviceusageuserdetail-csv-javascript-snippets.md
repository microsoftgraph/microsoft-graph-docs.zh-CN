---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c3b4ef413d279d21fb696f8bad15e2495b223021
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```