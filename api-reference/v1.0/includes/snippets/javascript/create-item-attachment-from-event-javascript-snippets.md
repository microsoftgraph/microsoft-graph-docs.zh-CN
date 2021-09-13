---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17601462cad1deaadbb64c9a5e73ae065f545a8abed3cbb01f9658d50713029c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332604"
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