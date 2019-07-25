---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 918d73c1863df00e4b4f473a154ae77d6b17b232
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarview/delta?startdatetime=%7Bstart_datetime%7D&enddatetime=%7Bend_datetime%7D')
    .version('beta')
    .get();

```