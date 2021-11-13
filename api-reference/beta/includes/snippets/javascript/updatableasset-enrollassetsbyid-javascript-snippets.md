---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ea08db58deccbb7047297e3e97394a97255305c61d5b290492108985aea14a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332464"
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