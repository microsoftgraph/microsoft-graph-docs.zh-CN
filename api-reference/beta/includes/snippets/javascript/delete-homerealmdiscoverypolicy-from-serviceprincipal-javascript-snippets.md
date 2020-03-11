---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e4c212cafa2bbd7d3ab6d96beb418d4b96d09bb
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref')
    .version('beta')
    .delete();

```