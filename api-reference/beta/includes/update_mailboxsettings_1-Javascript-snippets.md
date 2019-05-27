---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c22dd0cd41dd1569254a243b7092aa1967f4c59
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
    @odata.context: "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    automaticRepliesSetting: {
        status: "Scheduled",
        scheduledStartDateTime: {
          dateTime: "2016-03-20T18:00:00.0000000",
          timeZone: "UTC"
        },
        scheduledEndDateTime: {
          dateTime: "2016-03-28T18:00:00.0000000",
          timeZone: "UTC"
        }
    }
};

let res = await client.api('/me/mailboxSettings')
    .version('beta')
    .update({mailboxSettings : mailboxSettings});

```