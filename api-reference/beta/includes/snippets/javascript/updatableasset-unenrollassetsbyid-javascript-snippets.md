---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfdf0f463f0d1caeb7533410f4834edd890057fa
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240691"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unenrollAssetsById = {
  updateCategory: 'feature',
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice',
  ids: [
    'String',
    'String',
    'String'
  ]
};

await client.api('/admin/windows/updates/updatableAssets/unenrollAssetsById')
    .version('beta')
    .post(unenrollAssetsById);

```