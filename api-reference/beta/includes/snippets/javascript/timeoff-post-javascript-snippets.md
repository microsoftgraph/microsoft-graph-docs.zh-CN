---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a769b644b51e5fa91a0fe0d9f756d9418f1c973d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718120"
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
    .post({timeOff : timeOff});

```