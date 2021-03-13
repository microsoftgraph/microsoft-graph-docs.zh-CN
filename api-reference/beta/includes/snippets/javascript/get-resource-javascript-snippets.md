---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51c8622d73a70b924eb34b6f3bbb9fe1857a8e7f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/onenote/resources/{id}/content')
    .version('beta')
    .get();

```