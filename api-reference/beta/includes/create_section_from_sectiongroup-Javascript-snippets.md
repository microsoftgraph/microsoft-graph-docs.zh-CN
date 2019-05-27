---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 052e68ff451e47635264acf4bf91cfaea7d08edf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439573"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .post({onenoteSection : onenoteSection});

```