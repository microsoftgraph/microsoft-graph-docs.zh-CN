---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 328bbee916fd6f37e220913b924f2069420c09a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/me/createdObjects')
    .version('beta')
    .get();

```