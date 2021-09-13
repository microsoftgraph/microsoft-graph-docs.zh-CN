---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51e534025200a2338743247a7a92a42c0f0773ccecce1827a8cae4e729f6f595
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162942"
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