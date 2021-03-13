---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad9f965f42b68b0721729f7c12160dc2b050d62
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const shift = {
  id: 'SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8',
  userId: 'c5d0c76b-80c4-481c-be50-923cd8d680a1',
  schedulingGroupId: 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0',
  sharedShift: {
    displayName: 'Day shift',
    notes: 'Please do inventory as part of your shift.',
    startDateTime: '2019-03-11T15:00:00Z',
    endDateTime: '2019-03-12T00:00:00Z',
    theme: 'blue',
    activities: [
      {
        isPaid: true,
        startDateTime: '2019-03-11T15:00:00Z',
        endDateTime: '2019-03-11T15:15:00Z',
        code: '',
        displayName: 'Lunch'
      }
    ]
  },
  draftShift: {
    displayName: 'Day shift',
    notes: 'Please do inventory as part of your shift.',
    startDateTime: '2019-03-11T15:00:00Z',
    endDateTime: '2019-03-12T00:00:00Z',
    theme: 'blue',
    activities: [
      {
        isPaid: true,
        startDateTime: '2019-03-11T15:00:00Z',
        endDateTime: '2019-03-11T15:30:00Z',
        code: '',
        displayName: 'Lunch'
      }
    ]
  }
};

await client.api('/teams/{teamId}/schedule/shifts')
    .version('beta')
    .post(shift);

```