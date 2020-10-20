---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0abad1f53cd3962ce4fb12d14f7d3d0f713796c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/resources/{id}/content')
    .version('beta')
    .get();

```