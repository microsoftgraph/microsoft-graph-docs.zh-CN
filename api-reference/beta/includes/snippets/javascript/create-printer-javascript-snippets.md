---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 500da7383df80c7aa68f8122e114b86238e45e3f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const create = {
  displayName: "Test Printer",
  manufacturer: "Test Printer Manufacturer",
  model: "Test Printer Model",
  physicalDeviceId: null,
  hasPhysicalDevice: false,
  certificateSigningRequest: { 
    content: "{content}",
    transportKey: "{sampleTransportKey}"
  },
  connectorId: null
};

let res = await client.api('/print/printers/create')
    .version('beta')
    .post(create);

```