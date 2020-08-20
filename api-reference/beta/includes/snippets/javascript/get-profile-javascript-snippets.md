---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75562cea0f468872a85a398bbe5e5f325d99bf17
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile')
    .version('beta')
    .expand('skills($select=displayName)')
    .get();

```