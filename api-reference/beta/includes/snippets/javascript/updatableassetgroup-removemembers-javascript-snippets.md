---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 153b87c0b844adcf3077cee3b7c3073ea9f6a53e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeMembers = {
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers')
    .version('beta')
    .post(removeMembers);

```