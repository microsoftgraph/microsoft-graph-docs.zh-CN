---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b9cb38610a8ea34b91de4d8297af293fc9c368da162826cce645d19f0ddc302
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103806"
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