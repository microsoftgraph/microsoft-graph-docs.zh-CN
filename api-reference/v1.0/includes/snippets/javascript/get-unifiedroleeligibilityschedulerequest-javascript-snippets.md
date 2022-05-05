---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc5cf26f0314dd2d649d444de874def7530d34e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleRequest = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/f341269e-c926-41fa-a905-cef3b01b2a67')
    .get();

```