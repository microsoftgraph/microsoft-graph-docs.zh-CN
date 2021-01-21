---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9189dd751ef20a64da263ec5b13eb009f8e67761
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegration = {
  displayName: "displayName-value",
  apiVersion: 99,
  encryption: {
    protocol: "protocol-value",
    secret: "secret-value"
  },
  isActive: true,
  url: "url-value",
  supportedEntities: "supportedEntities-value"
};

let res = await client.api('/teamwork/workforceIntegrations/{workforceIntegrationId}')
    .update(workforceIntegration);

```