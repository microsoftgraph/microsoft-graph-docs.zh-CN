---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 004896893bfa012cc40eda68442ba2d7572b97e1452a39093157a57e7815d425
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAssets = await client.api('/admin/windows/updates/updatableAssets/')
    .version('beta')
    .filter('isof(\'microsoft.graph.windowsUpdates.updatableAssetGroup\')')
    .get();

```