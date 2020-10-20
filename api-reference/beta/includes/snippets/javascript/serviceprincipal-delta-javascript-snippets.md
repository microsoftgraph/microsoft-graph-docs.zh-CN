---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7db48d9ce03407aa90d82f0256322371c2e7c019
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/delta')
    .version('beta')
    .get();

```