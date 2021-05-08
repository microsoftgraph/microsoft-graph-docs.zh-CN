---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cccbc6176a0c34f336bb9f0a2f2dba6849f25c8
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeMembersById = {
  ids: [
    'String',
    'String',
    'String'
  ],
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice'
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById')
    .version('beta')
    .post(removeMembersById);

```