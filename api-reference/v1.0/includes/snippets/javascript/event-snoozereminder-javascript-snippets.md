---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c2601cf72fa5df0449afafdd140a14675cb10d4695f59ac74ce64604bc960e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: 'dateTime-value',
    timeZone: 'timeZone-value'
  }
};

await client.api('/me/events/{id}/snoozeReminder')
    .post(snoozeReminder);

```