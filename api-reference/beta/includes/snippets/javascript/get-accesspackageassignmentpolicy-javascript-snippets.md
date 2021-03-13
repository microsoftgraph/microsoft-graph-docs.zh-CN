---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c343ed24274cd4f3bb5badb8eaed8b95ee698689
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentPolicy = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}')
    .version('beta')
    .get();

```