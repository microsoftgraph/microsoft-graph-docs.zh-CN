---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 837d28cf62cfa7fe9f44eb9454c58645822953ceca08d5fa3b3800cab667396f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: '2016-10-19T10:37:00Z',
    timeZone: 'timeZone-value'
  }
};

await client.api('/me/events/{id}/snoozeReminder')
    .version('beta')
    .post(snoozeReminder);

```