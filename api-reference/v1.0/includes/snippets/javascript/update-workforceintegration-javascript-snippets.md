---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef5cb7ee26dd4e7e10e3b77cc1c0dc9c469bb0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809439"
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