---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 832fd1c0d995a0d9c79e764a7178d4eccd13c39bf2f1fb038ab035a953f3c908
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentSchedule = await client.api('/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413')
    .version('beta')
    .get();

```