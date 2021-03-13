---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c3ba4f6629aa061cd07c2bb637394bfec10ee73
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/groups/{groupId}/drive')
    .version('beta')
    .get();

```