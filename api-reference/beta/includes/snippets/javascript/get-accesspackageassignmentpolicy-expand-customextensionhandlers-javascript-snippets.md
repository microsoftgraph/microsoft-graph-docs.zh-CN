---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81b63041b62619e97f9599fa6936420450392253
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentPolicy = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197')
    .version('beta')
    .expand('customExtensionHandlers($expand=customExtension)')
    .get();

```