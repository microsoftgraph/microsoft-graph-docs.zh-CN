---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20d71821e77ca22ad8402468f6acdf4e1d674ba83d8a1ce843e4f60b47fdc36c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleRequest = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}')
    .version('beta')
    .get();

```