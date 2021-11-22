---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef6535ffe01c8919d4729e103c2f4cbb07f4c25d23b65dbedc22d6998f815070
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221063"
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
  supports: 'supports-value'
};

await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .post(workforceIntegration);

```