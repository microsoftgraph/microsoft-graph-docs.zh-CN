---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f40e2d9d89689b11d2e9114a2b84d4a6b49c67d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788514"
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
    .post(share);

```