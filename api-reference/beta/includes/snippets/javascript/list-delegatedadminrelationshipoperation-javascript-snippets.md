---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6edd02be8b8aeff57590d749881b351f1e1dc58f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/operations')
    .version('beta')
    .get();

```