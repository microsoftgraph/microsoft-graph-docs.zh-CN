---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bbea6e0c8bea560170613bf96530129c503c6c0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAudience = {
  addMembers: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ],
  removeMembers: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ],
  addExclusions: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ],
  removeExclusions: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience')
    .version('beta')
    .post(updateAudience);

```