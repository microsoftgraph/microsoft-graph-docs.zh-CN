---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46ca1a5492c0307226a933f9ecfb560962973098
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .delete();

```