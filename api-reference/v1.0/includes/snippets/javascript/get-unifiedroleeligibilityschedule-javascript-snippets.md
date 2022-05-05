---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89ce75fa8170d5df21f880c64a8ff73d3ec0e2ef
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilitySchedule = await client.api('/roleManagement/directory/roleEligibilitySchedules/1f06eafc-7532-429b-abf1-ab5a5f4a7052')
    .get();

```