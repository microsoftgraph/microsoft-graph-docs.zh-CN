---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ce364ebcb188b54bdb3c5370f6774f7269f2f1079f629c29fd58bc56e4b3329
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215930"
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

await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .update(workforceIntegration);

```