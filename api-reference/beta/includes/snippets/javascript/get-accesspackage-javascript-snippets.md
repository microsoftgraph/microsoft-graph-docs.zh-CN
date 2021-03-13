---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43767c47ea26b6bf5b0e117be8d5d6d1bf6e2e45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackage = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .get();

```