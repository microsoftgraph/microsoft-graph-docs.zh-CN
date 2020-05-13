---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05ec196b56cae647d89acdb7eaa2dd2d1306923d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .version('beta')
    .delete();

```