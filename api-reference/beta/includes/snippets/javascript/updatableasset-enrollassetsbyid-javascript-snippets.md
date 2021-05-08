---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33ff00d5ec59d88c1c49002943ef124ae9123042
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const enrollAssetsById = {
  updateCategory: 'feature',
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice',
  ids: [
    'String',
    'String',
    'String'
  ]
};

await client.api('/admin/windows/updates/updatableAssets/enrollAssetsById')
    .version('beta')
    .post(enrollAssetsById);

```