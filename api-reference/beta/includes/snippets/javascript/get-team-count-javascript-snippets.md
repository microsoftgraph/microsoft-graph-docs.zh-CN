---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72e0fc2f7ed78b672b3208301a1789380aabc62c
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipals = await client.api('/servicePrincipals')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Team')
    .get();

```