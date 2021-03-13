---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bab12e866f51a312dea01dc9e34be1d67901562
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscriptions = await client.api('/subscriptions')
    .version('beta')
    .get();

```