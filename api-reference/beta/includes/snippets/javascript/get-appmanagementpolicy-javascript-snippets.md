---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33696ff6c07d70739595f494474a9a38a1aec7b8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appManagementPolicy = await client.api('/policies/appManagementPolicies/{id}')
    .version('beta')
    .get();

```