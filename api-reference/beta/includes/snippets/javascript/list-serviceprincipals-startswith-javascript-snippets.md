---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9243d9aa2543586330e095235fae034d16fbe6d6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .orderby('displayName')
    .top(1)
    .get();

```