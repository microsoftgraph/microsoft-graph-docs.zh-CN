---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab9d032822276a307e1aa429920d5e0f2da1c744
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800669"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSku = await client.api('/subscribedSkus/{id}')
    .version('beta')
    .get();

```