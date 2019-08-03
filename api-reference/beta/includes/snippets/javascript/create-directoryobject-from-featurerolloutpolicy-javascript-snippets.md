---
description: 自动生成的文件。 不修改
ms.openlocfilehash: befec520fd3342c64171412ec5ff0e0c61e256bb
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
};

let res = await client.api('/directory/featureRolloutPolicies/{id}/appliesTo/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```