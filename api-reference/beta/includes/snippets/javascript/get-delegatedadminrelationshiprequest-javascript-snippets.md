---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6664c3bd670664048b77614ad8f2a150948ad207
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminRelationshipRequest = await client.api('/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests/cf4a23c7-070c-4d1c-8be8-1e86085ac9d1')
    .version('beta')
    .get();

```