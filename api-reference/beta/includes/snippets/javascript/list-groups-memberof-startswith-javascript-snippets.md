---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b99ec0e0ee0791cc24e7e11a0eaa6b0592ef6e2f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/memberOf/microsoft.graph.group')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'A\')')
    .orderby('displayName')
    .get();

```