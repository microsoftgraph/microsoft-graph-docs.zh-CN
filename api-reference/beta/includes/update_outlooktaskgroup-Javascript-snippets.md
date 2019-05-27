---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fedfe76fee1e7b3b970f67df8529bb3d115b3a89
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: "Personal Tasks",
};

let res = await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .update({outlookTaskGroup : outlookTaskGroup});

```