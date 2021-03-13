---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afaa3077be1fd16171a8a5680ea0ad7a4f3ab5f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const create = {
  displayName: 'Test Printer',
  manufacturer: 'Test Printer Manufacturer',
  model: 'Test Printer Model',
  physicalDeviceId: null,
  hasPhysicalDevice: false,
  certificateSigningRequest: { 
    content: '{content}',
    transportKey: '{sampleTransportKey}'
  },
  connectorId: null
};

await client.api('/print/printers/create')
    .version('beta')
    .post(create);

```