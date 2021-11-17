---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 530341bdbc2924580c9aa60876c288dd5a0bb52192a9c42fa343aadb1acfdfc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicy);

```