---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4da4e2915e265d84d363d7d71484c618d1877863
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let orgContact = await client.api('/contacts/{id}')
    .version('beta')
    .get();

```