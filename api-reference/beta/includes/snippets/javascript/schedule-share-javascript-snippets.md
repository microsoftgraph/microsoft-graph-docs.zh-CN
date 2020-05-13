---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6d2fb21c9c8e0bf4de45469c3d0e698bf88ec67
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35718099"
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