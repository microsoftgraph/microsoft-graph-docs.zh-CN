---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9f1f89fa9b065f27fac6682632c2cd3533f5fe1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/groups/{id}/transitiveMembers/microsoft.graph.user')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .orderby('displayName')
    .get();

```