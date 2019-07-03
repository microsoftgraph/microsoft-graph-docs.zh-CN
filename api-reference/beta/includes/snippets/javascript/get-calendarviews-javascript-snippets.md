---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 910a8ac5869ae21b6c37cee87c765b2d53a631f7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00')
    .version('beta')
    .header('Prefer','outlook.body-content-type="text"')
    .get();

```