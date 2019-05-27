---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 594379190675422c4cc4ce3f9409e4e9b5b8e8c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .get();

```