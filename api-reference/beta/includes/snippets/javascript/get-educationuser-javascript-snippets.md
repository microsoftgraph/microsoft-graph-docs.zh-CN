---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d58dffac4f7a336c401ab428d83615bc55f59618
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .version('beta')
    .get();

```