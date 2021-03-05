---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 802407753a4b7cc756c6e62efc4831d0d3c5761b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474752"
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
             dateTime: '2020-01-12T18:00:00',
             timeZone: 'Pacific Standard Time'
          },
          end: {
             dateTime: '2020-01-12T19:00:00',
             timeZone: 'Pacific Standard Time'
          }
    }
};

await client.api('/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments')
    .version('beta')
    .post(attachment);

```