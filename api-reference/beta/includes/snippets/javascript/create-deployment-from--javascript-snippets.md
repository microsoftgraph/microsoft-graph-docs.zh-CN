---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06c0ed4a8b72e5f725851d4c1859370c8579e30f6e01f594e462fb5edcc71450
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104468"
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