---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bd429ae8c95d032d8998b1b2f415e743035ff44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let alerts = await client.api('/security/alerts')
    .version('beta')
    .get();

```