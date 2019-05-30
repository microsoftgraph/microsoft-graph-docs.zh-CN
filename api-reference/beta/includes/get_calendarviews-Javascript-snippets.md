---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 910a8ac5869ae21b6c37cee87c765b2d53a631f7
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536636"
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