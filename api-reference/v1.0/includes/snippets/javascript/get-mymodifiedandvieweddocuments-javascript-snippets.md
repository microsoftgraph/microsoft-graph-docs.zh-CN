---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313a4d66e4d92b4b1e790cb1a9148c8b34d39fc7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .orderby('LastUsed/LastAccessedDateTime desc')
    .get();

```