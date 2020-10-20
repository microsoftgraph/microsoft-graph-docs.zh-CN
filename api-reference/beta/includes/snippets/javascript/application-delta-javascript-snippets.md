---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a288ed7f335a04247fbca11a2da80db607076b6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616912"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/delta')
    .version('beta')
    .get();

```