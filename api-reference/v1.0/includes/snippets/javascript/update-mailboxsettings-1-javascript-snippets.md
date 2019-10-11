---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ede46641a7fdb9bf4e74945944b940ab9032e50c
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailboxSettings = {
    @odata.context: "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
    .update(mailboxSettings);

```