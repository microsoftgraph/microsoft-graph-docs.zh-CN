---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a868964aa66c69bbf9c7e222993cdda24512d1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .filter('scopeId eq \'/\' and scopeType eq \'DirectoryRole\'')
    .get();

```