---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5509185531bc885d212ceda422ca02161507f0f8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const informationProtectionAction = {
  contentInfo: {
    @odata.type: "#microsoft.graph.contentInfo",
    format@odata.type: "#microsoft.graph.contentFormat",
    format: "default",
    identifier: null,
    state@odata.type: "#microsoft.graph.contentState",
    state: "rest"
  },
  classificationResults: [
    {
      sensitiveTypeId: "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
      count: 4,
      confidenceLevel: 75
    }
  ]
};

let res = await client.api('/informationProtection/policy/labels/evaluateClassificationResults')
    .version('beta')
    .post(informationProtectionAction);

```