---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a624531dd795e5a00976e945f04ad22b6b88966f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636632"
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
    .post(securityAction);

```