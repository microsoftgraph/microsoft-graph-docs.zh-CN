---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28f86ca675b7ee5bbd4ddc26f3ed58a0927a419e
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47331080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='Contoso Project')')
    .version('beta')
    .get();

```