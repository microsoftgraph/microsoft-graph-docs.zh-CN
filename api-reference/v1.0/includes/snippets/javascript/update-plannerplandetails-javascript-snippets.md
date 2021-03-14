---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a703173a8106297e91a3f3d0c0e8289d65c6901
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlanDetails = {
  sharedWith: {
    '6463a5ce-2119-4198-9f2a-628761df4a62': true,
    'd95e6152-f683-4d78-9ff5-67ad180fea4a': false,
  },
  categoryDescriptions: {
    category1: 'Indoors',
    category3: null,
  }
};

await client.api('/planner/plans/{plan-id}/details')
    .update(plannerPlanDetails);

```