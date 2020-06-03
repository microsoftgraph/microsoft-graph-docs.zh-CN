---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c4be15ee4be0247813491d617a263dba0cafe63
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const share = {
  notifyTeam: true,
  startDateTime: "2018-10-08T00:00:00.000Z",
  endDateTime: "2018-10-15T00:00:00.000Z"
};

let res = await client.api('/teams/{teamId}/schedule/share')
    .post(share);

```