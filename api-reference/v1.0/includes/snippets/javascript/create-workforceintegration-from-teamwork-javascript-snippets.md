---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8da0a55ddc2102546604b8b22558498aa7289b3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218242"
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

let res = await client.api('/teamwork/workforceIntegrations')
    .post(workforceIntegration);

```