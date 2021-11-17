---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64a19c1ea67a3a6ef05aa33bab6eb2f5339af86edeae03d60c4023ed56ed03c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addMembersById = {
  ids: [
    'String',
    'String',
    'String'
  ],
  memberEntityType: '#microsoft.graph.windowsUpdates.azureADDevice'
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById')
    .version('beta')
    .post(addMembersById);

```