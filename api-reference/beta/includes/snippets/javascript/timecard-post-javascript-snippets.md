---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f318686857db24886ae585e9aa2f66994fe59ec3
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeCard = {
  onBehalfOfUserId: 'a3601044-a1b5-438e-b742-f78d01d68a67',
  clockInEvent: {
     dateTime: '2019-03-18T00:00:00.000Z',
     atApprovedLocation: true,
     notes: {
        content: 'Started late due to traffic in CA 237',
        contentType: 'text'
     },
  },
  notes: {
        content: '8 To 5 Inventory management',
        contentType: 'text'
   },
  breaks: [
     {
       breakId: 'string',
        notes: {
             content: 'Lunch break',
             contentType: 'text'
        },
        start: {
           dateTime: '2019-03-18T02:00:00.000Z',
           atApprovedLocation: true,
           notes: {
                content: 'Reduced break to make up for lost time',
                contentType: 'text'
             },
        }
     }
  ]
};

await client.api('/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards')
    .version('beta')
    .post(timeCard);

```