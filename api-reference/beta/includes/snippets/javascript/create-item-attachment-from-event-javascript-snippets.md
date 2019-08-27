---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e67a0d11d2e33d40e23f770b988b45abccf571a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633235"
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

let res = await client.api('/me/events/{AAMkAGI1AAAt9AHjAAA=}/attachments')
    .version('beta')
    .post(attachment);

```