---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 022a3f68ec0e83c4fa0a3572984fa6f3b25ec3f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .get();

```