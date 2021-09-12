---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c8e2a8e04826c972d3863bd4f0b79b989ed755835eb3a807f5a8b428311a3fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904298"
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