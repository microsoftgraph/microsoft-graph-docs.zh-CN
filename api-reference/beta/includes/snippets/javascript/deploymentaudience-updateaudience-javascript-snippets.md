---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37f2d4bf0bd5650e98f5d13e52c7a4721eb53e4bdc7c3267d8ac58fb5c8d7899
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378371"
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