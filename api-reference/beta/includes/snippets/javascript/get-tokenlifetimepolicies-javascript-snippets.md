---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98ba91cb984eef6a65d4f8ab333dbdeb19e6863b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .get();

```