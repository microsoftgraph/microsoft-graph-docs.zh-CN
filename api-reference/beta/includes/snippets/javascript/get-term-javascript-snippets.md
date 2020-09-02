---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7422d7ae380ebdea023977058ea172d189e06630
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/sets/{setId}/children')
    .version('beta')
    .get();

```