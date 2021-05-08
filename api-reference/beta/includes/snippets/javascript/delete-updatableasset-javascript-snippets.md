---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eec3c218684082dd73dfcc603f33788bff72a4b4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240727"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetId}')
    .version('beta')
    .delete();

```