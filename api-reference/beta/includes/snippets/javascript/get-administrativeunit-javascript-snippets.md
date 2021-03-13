---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d0ce470ce24e3e99f71780b61efc07e151ef78f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnit = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .get();

```