---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fc38252c1853f67c10708559cc585ea0829103ec3031fcc92b9997bc4c3de03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278264"
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