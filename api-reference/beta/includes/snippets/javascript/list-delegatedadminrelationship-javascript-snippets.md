---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fe1e162437ef5dcb25809e4628dc5a426611012
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminRelationships = await client.api('/tenantRelationships/delegatedAdminRelationships')
    .version('beta')
    .get();

```