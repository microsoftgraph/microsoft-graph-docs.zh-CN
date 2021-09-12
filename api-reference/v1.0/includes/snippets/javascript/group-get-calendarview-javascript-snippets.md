---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db4f881283a85b3907e6b754d8aa2354afd660418b3302f0fd6519d01f5f9be2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00')
    .header('Prefer','outlook.body-content-type="text"')
    .get();

```