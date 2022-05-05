---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9acedf96cb9217ee2aaa4a1aadecbabb67c310
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser(on='principal')')
    .get();

```