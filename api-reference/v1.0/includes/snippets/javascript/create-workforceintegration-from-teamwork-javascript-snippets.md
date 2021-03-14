---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38168da757d59292d7cc9c03dc6fd5ff3ce53ed7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783815"
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