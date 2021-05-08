---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 109aa2257f3a0220b7e7e50156db795a15633317
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238439"
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