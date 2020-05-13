---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ad35fa3013e96b78321078c2628b3acc001961b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "36636680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const shift = {
  id: "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  createdDateTime: "2019-03-14T04:32:51.451Z",
  lastModifiedDateTime: "2019-03-14T05:32:51.451Z",
  userId: "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  schedulingGroupId: "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  lastModifiedBy: {
    application: null,
    device: null,
    conversation: null,
    user: {
      id: "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      displayName: "John Doe"
    }
  },
  sharedShift: {
    displayName: "Day shift",
    notes: "Please do inventory as part of your shift.",
    startDateTime: "2019-03-11T15:00:00Z",
    endDateTime: "2019-03-12T00:00:00Z",
    theme: "blue",
    activities: [
      {
        isPaid: true,
        startDateTime: "2019-03-11T15:00:00Z",
        endDateTime: "2019-03-11T15:15:00Z",
        code: "",
        displayName: "Lunch"
      }
    ]
  },
  draftShift: {
    displayName: "Day shift",
    notes: "Please do inventory as part of your shift.",
    startDateTime: "2019-03-11T15:00:00Z",
    endDateTime: "2019-03-12T00:00:00Z",
    theme: "blue",
    activities: [
      {
        isPaid: true,
        startDateTime: "2019-03-11T15:00:00Z",
        endDateTime: "2019-03-11T15:30:00Z",
        code: "",
        displayName: "Lunch"
      }
    ]
  }
};

let res = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .put(shift);

```