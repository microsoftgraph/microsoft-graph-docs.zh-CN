---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfc0581d8b29c926773d9b3baedf49533f88a371
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636505"
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
    .post(directoryObject);

```