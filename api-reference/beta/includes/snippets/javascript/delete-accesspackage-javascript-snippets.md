---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d342bd3df2f3b5806f573f07365f29f3a7187e2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .delete();

```