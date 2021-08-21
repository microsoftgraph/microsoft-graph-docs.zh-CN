---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bccf0332b9569ecdea92d5e8f738bdeb2e9a0b6efb0a0a6a2342b8a4e00626f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel')
    .version('beta')
    .post();

```