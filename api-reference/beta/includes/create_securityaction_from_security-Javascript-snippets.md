---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 660cc6e0bd64a55c181d6aa3c7363b0ce31c3212
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const securityAction = {
  name: "BlockIp",
  actionReason: "Test",
  parameters: [
    {
      name: "IP",
      value: "1.2.3.4"
    }
  ],
  vendorInformation: {
    provider: "Windows Defender ATP",
    vendor: "Microsoft"
  }
};

let res = await client.api('/security/securityActions')
    .version('beta')
    .post({securityAction : securityAction});

```