---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1524d024b224ced14431d433e03a26fe0cf5130d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnits = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```