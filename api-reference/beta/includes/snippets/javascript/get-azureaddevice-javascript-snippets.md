---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 257c8d7e94c305903e8ea0ba4641ed887b3342ab
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAsset = await client.api('/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98')
    .version('beta')
    .get();

```