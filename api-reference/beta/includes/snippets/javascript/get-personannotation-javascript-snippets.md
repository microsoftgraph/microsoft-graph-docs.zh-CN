---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 960c7feb645b5399c339ec3b36f853e4a1d98e53
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/notes/{id}')
    .version('beta')
    .get();

```