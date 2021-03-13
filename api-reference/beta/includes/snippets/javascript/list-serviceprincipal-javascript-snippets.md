---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bd6f6fb12c982781a71c14f3e6049acac205e3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .get();

```