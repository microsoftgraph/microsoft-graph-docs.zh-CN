---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 606ff293ab204dcf81f1fc7e7c98b483e678501126bc718952e904d000356c03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329068"
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
  }
};

await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```