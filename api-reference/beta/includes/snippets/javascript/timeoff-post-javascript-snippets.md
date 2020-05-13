---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5edd2836fda8a2b449b19ebdcad09ab93a2127f6
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "36636636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOff = {
  userId: "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  sharedTimeOff: {
    timeOffReasonId: "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    startDateTime: "2019-03-11T07:00:00Z",
    endDateTime: "2019-03-12T07:00:00Z",
    theme: "white"
  },
  draftTimeOff: {
    timeOffReasonId: "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    startDateTime: "2019-03-11T07:00:00Z",
    endDateTime: "2019-03-12T07:00:00Z",
    theme: "pink"
  }
};

let res = await client.api('/teams/{teamId}/schedule/timesOff')
    .version('beta')
    .post(timeOff);

```