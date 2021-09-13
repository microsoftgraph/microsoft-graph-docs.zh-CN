---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc55607553ad28cd8528352cec79d23a03ef1f21cbd3aad11971d4dc5961c168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  '@odata.id':'https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/servicePrincipals/{id}/claimsMappingPolicies/$ref')
    .post(claimsMappingPolicy);

```