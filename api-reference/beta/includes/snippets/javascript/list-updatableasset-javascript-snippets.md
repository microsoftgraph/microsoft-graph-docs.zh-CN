---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fe7296371d94ea0d574315326939d3ca8a78b86
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "61004292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members')
    .version('beta')
    .get();

```