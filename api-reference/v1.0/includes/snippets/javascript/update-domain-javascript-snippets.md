---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58bda33eb46509bcaddb78189f0ffedfeacb7233ad4026e1453ec802f9db69b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    'Email',
    'OfficeCommunicationsOnline'
  ]
};

await client.api('/domains/contoso.com')
    .update(domain);

```