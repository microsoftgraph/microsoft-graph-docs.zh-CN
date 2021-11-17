---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61059a0181317ffba99731d0e010f4a14efadd1e08689a7019eb04b2a5a917f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentPolicies = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .get();

```