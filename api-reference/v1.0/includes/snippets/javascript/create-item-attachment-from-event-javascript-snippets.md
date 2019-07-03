---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e8c8938a9a3e59d19219e6465ece3fcbfe2c13c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467045"
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