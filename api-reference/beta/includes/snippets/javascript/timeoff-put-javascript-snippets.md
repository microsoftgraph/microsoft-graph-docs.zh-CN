---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bdb9ea7eea6d124a326885b1dc0654f16808b8d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOff = {
  userId: 'c5d0c76b-80c4-481c-be50-923cd8d680a1',
  sharedTimeOff: {
    timeOffReasonId: 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7',
    startDateTime: '2019-03-11T07:00:00Z',
    endDateTime: '2019-03-12T07:00:00Z',
    theme: 'white'
  },
  draftTimeOff: {
    timeOffReasonId: 'TOR_891045ca-b5d2-406b-aa06-a3c8921245d7',
    startDateTime: '2019-03-11T07:00:00Z',
    endDateTime: '2019-03-12T07:00:00Z',
    theme: 'pink'
  }
};

await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .put(timeOff);

```