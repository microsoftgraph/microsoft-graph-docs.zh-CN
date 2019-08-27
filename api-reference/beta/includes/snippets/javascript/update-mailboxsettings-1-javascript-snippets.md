---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcd74492d31bab0b1e6c968dc5be4a642b8d805f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636602"
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
    .update(mailboxSettings);

```