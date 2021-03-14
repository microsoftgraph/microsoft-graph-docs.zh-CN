---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b90243cf2bf7e758eaaeeaff85e1c92ed35c0dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
    '@odata.context': 'https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings',
    automaticRepliesSetting: {
        status: 'Scheduled',
        scheduledStartDateTime: {
          dateTime: '2016-03-20T18:00:00.0000000',
          timeZone: 'UTC'
        },
        scheduledEndDateTime: {
          dateTime: '2016-03-28T18:00:00.0000000',
          timeZone: 'UTC'
        }
    }
};

await client.api('/me/mailboxSettings')
    .update(mailboxSettings);

```