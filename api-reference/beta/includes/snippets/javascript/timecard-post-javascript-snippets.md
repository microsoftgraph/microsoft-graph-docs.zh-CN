---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a68c1005bf13adeb8cd74330b9561fa88fb94cfdec9c289bbc289c1484e062a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328908"
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