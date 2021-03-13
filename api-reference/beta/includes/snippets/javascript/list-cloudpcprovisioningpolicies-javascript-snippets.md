---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a45aa86b660a65623b0a1ea3daff4da6577d5e85
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let provisioningPolicies = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .get();

```