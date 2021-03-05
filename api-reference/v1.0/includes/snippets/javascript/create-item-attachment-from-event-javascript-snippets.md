---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05e4e672b7fefb70c77b17c3b596b18a30753535
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#microsoft.graph.itemAttachment',
  name: 'Holiday event', 
  item: {
        '@odata.type': 'microsoft.graph.event',
        subject: 'Discuss gifts for children',
        body: {
            contentType: 'HTML',
            content: 'Let\'s look for funding!'
         },
         start: {
             dateTime: '2016-12-02T18:00:00',
             timeZone: 'Pacific Standard Time'
          },
          end: {
             dateTime: '2016-12-02T19:00:00',
             timeZone: 'Pacific Standard Time'
          }
    }
};

await client.api('/me/events/AAMkAGI1AAAt9AHjAAA=/attachments')
    .post(attachment);

```