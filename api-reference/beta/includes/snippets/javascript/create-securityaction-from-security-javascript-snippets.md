---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a907c3eeba3c963473d0faced4d8fbb6b9b46654528af382412385bbf14ff203
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const securityAction = {
  name: 'BlockIp',
  actionReason: 'Test',
  parameters: [
    {
      name: 'IP',
      value: '1.2.3.4'
    }
  ],
  vendorInformation: {
    provider: 'Windows Defender ATP',
    vendor: 'Microsoft'
  }
};

await client.api('/security/securityActions')
    .version('beta')
    .post(securityAction);

```