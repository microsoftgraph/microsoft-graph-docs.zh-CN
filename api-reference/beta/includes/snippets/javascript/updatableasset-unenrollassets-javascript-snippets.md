---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5d2b09ba8d91701e5bcd4ae8c37f8fa4f4b4685
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442851"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unenrollAssets = {
  updateCategory: 'String',
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/unenrollAssets')
    .version('beta')
    .post(unenrollAssets);

```