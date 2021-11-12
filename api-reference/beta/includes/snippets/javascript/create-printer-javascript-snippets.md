---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95aefb13728e511b064102fca82fc274dbec93a5b315f928fe78ba8923643187
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902396"
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