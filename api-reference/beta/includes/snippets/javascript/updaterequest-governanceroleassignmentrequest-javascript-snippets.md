---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e896cb9d4c9149f308abd0dbf46ebe3fb652de1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest')
    .version('beta')
    .post();

```