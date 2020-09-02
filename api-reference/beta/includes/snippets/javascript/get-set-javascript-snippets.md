---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72020900fac104db90047f8f9832366a23e9a419
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/sets/{setId}')
    .version('beta')
    .get();

```