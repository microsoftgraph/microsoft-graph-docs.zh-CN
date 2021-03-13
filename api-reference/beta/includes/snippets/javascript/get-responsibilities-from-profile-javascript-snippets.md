---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 891e744360c37b90c0b1c89be899e37145312489
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let responsibilities = await client.api('/me/responsibilities')
    .version('beta')
    .get();

```