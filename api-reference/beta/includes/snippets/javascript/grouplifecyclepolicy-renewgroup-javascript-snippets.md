---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4259a99133c75013f77a921c5dc8670ffbd28da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  groupId: 'ffffffff-ffff-ffff-ffff-ffffffffffff'
};

await client.api('/groupLifecyclePolicies/renewGroup')
    .version('beta')
    .post(_boolean);

```