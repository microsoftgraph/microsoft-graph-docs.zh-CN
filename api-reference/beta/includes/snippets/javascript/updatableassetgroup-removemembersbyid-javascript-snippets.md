---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e65ae3da5013a850cc80008598b8322b4184f1c94072be2f7423af01bf9abdd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219513"
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