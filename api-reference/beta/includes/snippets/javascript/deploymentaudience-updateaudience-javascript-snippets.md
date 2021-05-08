---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3418cf84cc9944df3bf7744ac8c4e0979f8b8a2a
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAudience = {
  addMembers: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.updatableAsset',
      id: 'String (identifier)'
    }
  ],
  removeMembers: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.updatableAsset',
      id: 'String (identifier)'
    }
  ],
  addExclusions: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.updatableAsset',
      id: 'String (identifier)'
    }
  ],
  removeExclusions: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.updatableAsset',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience')
    .version('beta')
    .post(updateAudience);

```