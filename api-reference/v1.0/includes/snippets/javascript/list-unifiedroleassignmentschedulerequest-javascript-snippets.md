---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99266389c3062b28bd01bad14c357c771bf1fa43
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentScheduleRequests = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests')
    .get();

```