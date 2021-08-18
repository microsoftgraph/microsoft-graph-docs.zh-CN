---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 613c3b2aedd7e12104ac71eeaf5305afa721ab03
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/appManagementPolicies/{id}/appliesTo')
    .version('beta')
    .get();

```