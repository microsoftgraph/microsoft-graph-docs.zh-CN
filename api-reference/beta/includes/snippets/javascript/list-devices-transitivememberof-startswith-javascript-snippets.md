---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d433cee83d95697d7c0023648abd9b6050f0a63
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/devices/{id}/transitiveMemberOf/microsoft.graph.group')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .orderby('displayName')
    .get();

```