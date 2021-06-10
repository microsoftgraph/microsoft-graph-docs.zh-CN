---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad4e9ffd43014a3a98e0ee49b41557df527c8052
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deployment = {
  '@odata.type': '#microsoft.graph.windowsUpdates.deployment',
  state: {
    '@odata.type': 'microsoft.graph.windowsUpdates.deploymentState',
    requestedValue: 'paused'
  },
};

await client.api('/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5')
    .version('beta')
    .update(deployment);

```