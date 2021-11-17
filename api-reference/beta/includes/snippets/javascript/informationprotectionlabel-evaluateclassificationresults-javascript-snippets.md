---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f487e8429fd133d266e9df21e77ab8e681d083908f21694779c4e9fa28acc882
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332494"
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