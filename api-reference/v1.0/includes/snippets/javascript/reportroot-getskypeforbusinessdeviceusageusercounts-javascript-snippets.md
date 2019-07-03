---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14f7d6c8041bc61af282b07eac292fd70ccbc3d6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')')
    .get();

```