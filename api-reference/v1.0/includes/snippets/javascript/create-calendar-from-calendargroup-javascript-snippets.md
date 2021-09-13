---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8caf2501f97a3dd2da7e09977d45aa65b69f4f9c646ca28f078d259c88e9a8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332132"
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
    .post(calendar);

```