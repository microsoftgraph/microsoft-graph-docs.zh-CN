---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75e86664fd0770db8f0cbdf6413e44924624b836
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "40870452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegrations = {
  displayName: "displayName-value",
  apiVersion: 99,
  encryption: {
    protocol: "protocol-value",
    secret: "secret-value"
  },
  isActive: true,
  url: "url-value",
  supports: "supports-value"
};

let res = await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .update(workforceIntegrations);

```