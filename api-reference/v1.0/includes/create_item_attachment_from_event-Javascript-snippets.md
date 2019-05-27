---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e8c8938a9a3e59d19219e6465ece3fcbfe2c13c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460697"
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

let res = await client.api('/me/events/AAMkAGI1AAAt9AHjAAA=/attachments')
    .post({attachment : attachment});

```