---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1926c033ec2165d4cc0b6fa5cdf2b6a1baca58f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
    '@odata.context': 'https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings',
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
    .version('beta')
    .update(mailboxSettings);

```