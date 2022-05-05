---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 580627dc6703d53cb367bd24b6bf52da5c1ef19e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/groups/{id}/transitiveMembers/microsoft.graph.user')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .orderby('displayName')
    .get();

```