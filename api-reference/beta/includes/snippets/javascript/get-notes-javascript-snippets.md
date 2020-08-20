---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 806664bfa6b5692b7abaf7342db5e62ac782bf7e
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819372"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/notes')
    .version('beta')
    .get();

```