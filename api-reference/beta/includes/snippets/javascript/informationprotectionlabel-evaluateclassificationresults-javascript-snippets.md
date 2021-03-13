---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d3b68d3b5b826c933b8dbc1c9ce75d3d0fcd60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const informationProtectionAction = {
  contentInfo: {
    '@odata.type': '#microsoft.graph.contentInfo',
    'format@odata.type': '#microsoft.graph.contentFormat',
    format: 'default',
    identifier: null,
    'state@odata.type': '#microsoft.graph.contentState',
    state: 'rest'
  },
  classificationResults: [
    {
      sensitiveTypeId: 'cb353f78-2b72-4c3c-8827-92ebe4f69fdf',
      count: 4,
      confidenceLevel: 75
    }
  ]
};

await client.api('/informationProtection/policy/labels/evaluateClassificationResults')
    .version('beta')
    .post(informationProtectionAction);

```