---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bc852de25f80b5a46987ebbb46d4c5de44bdf9b8a1080d8370232c9a42e8315
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  '@odata.id':'https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenIssuancePolicies/$ref')
    .post(tokenIssuancePolicy);

```