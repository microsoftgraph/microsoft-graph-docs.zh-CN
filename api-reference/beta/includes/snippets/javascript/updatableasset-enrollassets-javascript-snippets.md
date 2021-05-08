---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03b1339c5acaf26333dc4eb5cdb81f5824562eee
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const enrollAssets = {
  updateCategory: 'String',
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/enrollAssets')
    .version('beta')
    .post(enrollAssets);

```