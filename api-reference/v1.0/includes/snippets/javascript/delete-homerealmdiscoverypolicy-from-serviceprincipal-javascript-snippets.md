---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7782831414ded1cbc7318c848668f64561d0599
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref')
    .delete();

```