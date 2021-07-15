---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cf2499ccdce6378f5135cd48c4899dc6399e5bb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addMembers = {
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers')
    .version('beta')
    .post(addMembers);

```