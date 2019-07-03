---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a57fe33fe3c67d127c3fc194504ba583cbeede37
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.itemAttachment",
  name: "Holiday event", 
  item: {
    @odata.type: "microsoft.graph.event",
    subject: "Discuss gifts for children",
    body: {
      contentType: "HTML",
      content: "Let's look for funding!"
    },
    start: {
      dateTime: "2016-12-02T18:00:00",
      timeZone: "Pacific Standard Time"
    },
    end: {
      dateTime: "2016-12-02T19:00:00",
      timeZone: "Pacific Standard Time"
    }
  }
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post({attachment : attachment});

```