---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d296c19512de6a673a85077dceea1b6b2bc6f9
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/sets/{setId}')
    .version('beta')
    .delete();

```