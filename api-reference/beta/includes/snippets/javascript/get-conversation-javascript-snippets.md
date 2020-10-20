---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60cd1d4c1d13ebb7dda369ad8fa7506a531dae98
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .get();

```