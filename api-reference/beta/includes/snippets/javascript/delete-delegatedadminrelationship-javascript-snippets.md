---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98e96c67caacd5b945193c880f3f9f43bd187479
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836')
    .version('beta')
    .delete();

```