---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21211d84732e98fbf08a4b8f4a7db11656c0001e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  @odata.id:"https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/applications/{id}/tokenLifetimePolicies/$ref')
    .post(tokenLifetimePolicy);

```