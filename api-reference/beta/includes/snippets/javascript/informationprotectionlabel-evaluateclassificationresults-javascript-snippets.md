---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7b152babfecb70016cc78b650b39e426b43d06
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995618"
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