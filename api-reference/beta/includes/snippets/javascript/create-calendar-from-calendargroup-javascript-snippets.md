---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0688de6d5708098228a129ee30c617c58ab8b0bd67ac8752d1d209f6d4dadf3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Marketing calendar'
};

await client.api('/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars')
    .version('beta')
    .post(calendar);

```