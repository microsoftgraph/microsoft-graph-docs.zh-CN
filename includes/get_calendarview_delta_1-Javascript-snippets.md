---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8cff9f47239e09e570ab0c1af9a57a1893bed0d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34843827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```