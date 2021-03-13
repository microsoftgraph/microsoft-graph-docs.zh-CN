---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e7daa9d1be925653822e755f2be36461153db19
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printSettings = await client.api('/print/settings')
    .version('beta')
    .get();

```