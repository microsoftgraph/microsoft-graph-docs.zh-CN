---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b7451b978005ca476dc103210e74432024f833a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicies = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies')
    .get();

```