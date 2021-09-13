---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 033fbc0c7b9808f9483a02e36fd409eb402fe40232e58a4a4f0bd1c06e02c53e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  '@odata.id':'https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenLifetimePolicies/$ref')
    .post(tokenLifetimePolicy);

```