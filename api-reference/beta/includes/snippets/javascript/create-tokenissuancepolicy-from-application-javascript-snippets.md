---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2a5edcac76985bc4093a3fdfd13be9d62c51eb2
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  @odata.id:"https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/applications/{id}/tokenIssuancePolicies/$ref')
    .version('beta')
    .post(tokenIssuancePolicy);

```