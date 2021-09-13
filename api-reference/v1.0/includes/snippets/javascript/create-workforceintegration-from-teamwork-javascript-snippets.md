---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03d0144d9b02cb806cfbef9748856a42cc78082d39ea0300d2c8cb281ba914ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegration = {
  displayName: 'displayName-value',
  apiVersion: 99,
  encryption: {
    protocol: 'protocol-value',
    secret: 'secret-value'
  },
  isActive: true,
  url: 'url-value',
  supportedEntities: 'supportedEntities-value'
};

await client.api('/teamwork/workforceIntegrations')
    .post(workforceIntegration);

```