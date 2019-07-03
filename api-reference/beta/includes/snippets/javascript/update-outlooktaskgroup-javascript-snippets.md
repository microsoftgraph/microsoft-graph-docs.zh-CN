---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fedfe76fee1e7b3b970f67df8529bb3d115b3a89
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520112"
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