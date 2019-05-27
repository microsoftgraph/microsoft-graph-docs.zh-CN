---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe24d18c0dcc23884c36b07762ff14c6d21b182e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .version('beta')
    .post({sectionGroup : sectionGroup});

```