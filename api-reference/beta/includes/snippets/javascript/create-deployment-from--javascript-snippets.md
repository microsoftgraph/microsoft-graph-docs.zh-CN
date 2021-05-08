---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af343f08d9643172191ae8643989e5192b5529a6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deployment = {
  '@odata.type': '#microsoft.graph.windowsUpdates.deployment',
  content: {
    '@odata.type': 'microsoft.graph.windowsUpdates.featureUpdateReference',
    version: '20H2'
  },
  settings: {
    '@odata.type': 'microsoft.graph.windowsUpdates.windowsDeploymentSettings',
    rollout: {
      devicesPerOffer: 100
    },
    monitoring: {
      monitoringRules: [
        {
          '@odata.type': '#microsoft.graph.windowsUpdates.monitoringRule',
          signal: 'rollback',
          threshold: 5,
          action: 'pauseDeployment'
        }
      ]
    }
  }
};

await client.api('/admin/windows/updates/deployments')
    .version('beta')
    .post(deployment);

```