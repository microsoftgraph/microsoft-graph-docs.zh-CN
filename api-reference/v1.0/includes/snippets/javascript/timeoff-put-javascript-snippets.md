---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3406510eb6c3d2aae9e3c7d060a617168180ed5c6ca9a23a02cb036fea1bfa6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278194"
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
    .put(timeOff);

```