---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 737ec0cb85217aef579dd4b7ad88067ae6c5457f
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicies = {
  @odata.id:"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/applications/{id}/tokenLifetimePolicies')
    .version('beta')
    .post(tokenLifetimePolicies);

```