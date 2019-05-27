---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c6d2fb21c9c8e0bf4de45469c3d0e698bf88ec67
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480419"
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
    .version('beta')
    .post(share);

```