---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0a6c53023c6cc10109225f36e8ac0ecf2237301
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46644963"
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

let res = await client.api('/informationprotection/policy/labels/evaluateClassificationResults')
    .version('beta')
    .post(informationProtectionAction);

```