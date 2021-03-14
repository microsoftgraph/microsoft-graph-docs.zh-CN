---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bad049c635644bada13e88e7cba68314d4d0e245
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/me/presence')
    .get();

```