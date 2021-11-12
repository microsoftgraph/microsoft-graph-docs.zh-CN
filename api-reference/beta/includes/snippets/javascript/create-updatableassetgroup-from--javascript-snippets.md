---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72ecd7939b627bd5fbd841fb630cef9da5e9e00ef0e99e852ad0009b4ca46f57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updatableAsset = {
  '@odata.type': '#microsoft.graph.windowsUpdates.updatableAssetGroup'
};

await client.api('/admin/windows/updates/updatableAssets')
    .version('beta')
    .post(updatableAsset);

```