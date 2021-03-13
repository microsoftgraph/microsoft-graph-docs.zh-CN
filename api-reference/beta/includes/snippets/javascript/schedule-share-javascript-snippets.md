---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35502b43b5ebbd5c4a057dfa9cf9ec5626c7a9d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const share = {
  notifyTeam: true,
  startDateTime: '2018-10-08T00:00:00.000Z',
  endDateTime: '2018-10-15T00:00:00.000Z'
};

await client.api('/teams/{teamId}/schedule/share')
    .version('beta')
    .post(share);

```