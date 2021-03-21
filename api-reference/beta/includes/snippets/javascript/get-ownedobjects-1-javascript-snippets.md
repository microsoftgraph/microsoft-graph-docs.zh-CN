---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d2a06c67bd50c015f65c571d96bc877eca93f21
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/servicePrincipals/{id}/ownedObjects')
    .version('beta')
    .get();

```