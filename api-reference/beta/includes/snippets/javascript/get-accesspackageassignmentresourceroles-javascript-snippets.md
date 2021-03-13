---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 470e8a4e761a5c105caa8c6954d8e13f5533c172
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentResourceRoles = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles')
    .version('beta')
    .get();

```