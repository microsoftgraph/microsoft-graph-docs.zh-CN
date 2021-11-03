---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c99660e83788de1049785d7edb1e61a745528ee99f9e357c175cac0cac2424f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let steps = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps')
    .version('beta')
    .get();

```