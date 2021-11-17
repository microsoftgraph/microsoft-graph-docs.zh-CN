---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98d75f1f353714143702defb9715be36ceb7c434fa1bc04e493d00ae86b5836a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279496"
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