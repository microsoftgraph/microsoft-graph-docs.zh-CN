---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c39dde6360afb06801a7f77779afe18c5aa0cdf69c0dc9a27ca2112db5d54a07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333308"
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