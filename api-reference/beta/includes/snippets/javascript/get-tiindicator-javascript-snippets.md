---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df3594dcd696825e3a6875f257d41306aa9a81b9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tiIndicator = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .get();

```