---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a8943944d3fcccc445366b5b6ec241c12d7038e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z')
    .version('beta')
    .get();

```