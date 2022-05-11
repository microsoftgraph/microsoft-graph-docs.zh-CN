---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaac9622b4e23f7853b4838555bf7eede5d10150
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .filter('scopeId eq \'/\' and scopeType eq \'Directory\'')
    .expand('rules')
    .get();

```