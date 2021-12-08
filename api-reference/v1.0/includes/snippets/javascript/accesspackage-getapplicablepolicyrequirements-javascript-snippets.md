---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32b2741fff8c2f5a0c602aeed0e154dd1b1e97af
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}/getApplicablePolicyRequirements')
    .post();

```