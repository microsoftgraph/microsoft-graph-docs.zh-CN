---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56d6e52753a18d040510e4391f4b67305d4c2e8f
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  @odata.id:"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies/$ref')
    .post(claimsMappingPolicy);

```