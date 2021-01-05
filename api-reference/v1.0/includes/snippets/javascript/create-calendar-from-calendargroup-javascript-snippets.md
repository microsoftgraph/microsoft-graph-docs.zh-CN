---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f9601b03f30e663fa87663dfc2cab872c719efe
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Marketing calendar"
};

let res = await client.api('/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars')
    .post(calendar);

```