---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0376231a25dd99f1e5f49b27cb68bcb39304536f93042ad004c8289cfd482a34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let approvalStep = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095')
    .version('beta')
    .get();

```