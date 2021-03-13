---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d47420194feea6d47967e73e494c36a140423ae2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref')
    .version('beta')
    .delete();

```