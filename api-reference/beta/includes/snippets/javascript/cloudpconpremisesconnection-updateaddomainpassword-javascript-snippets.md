---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf5d18d65d79e1ede389d069775dd6034f298d51
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAdDomainPassword = {
  adDomainPassword: 'AdDomainPassword value'
};

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword')
    .version('beta')
    .update(updateAdDomainPassword);

```