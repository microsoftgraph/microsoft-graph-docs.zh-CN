---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a755c793a5b44a046d95a9645ad49b3d94f5902
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: 'default',
    identity: {
        phone: {
          '@odata.type': '#microsoft.graph.identity',
          id: '+12345678901'
        }
    },
    languageId: 'languageId-value',
    region: 'region-value'
  },
  clientContext: '9e90d1c1-f61e-43e7-9f75-d420159aae08'
};

await client.api('/communications/calls/{id}/transfer')
    .post(transfer);

```