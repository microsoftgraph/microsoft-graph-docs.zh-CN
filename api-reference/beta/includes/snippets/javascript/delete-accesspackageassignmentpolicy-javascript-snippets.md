---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 793a5df46b9a06ab496042faa9387fec4099fc50
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}')
    .version('beta')
    .delete();

```