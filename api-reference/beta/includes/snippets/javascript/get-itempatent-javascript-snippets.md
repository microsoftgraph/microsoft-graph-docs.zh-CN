---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e91e396ee7faf4ef601dbc972c2852b6b18ab1b9
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/patents/{id}')
    .version('beta')
    .get();

```