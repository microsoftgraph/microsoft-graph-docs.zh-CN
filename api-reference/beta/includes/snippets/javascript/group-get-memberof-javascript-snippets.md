---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b05d466b66d3e34fa689a780d74364198aade74d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/groups/{id}/memberOf')
    .version('beta')
    .get();

```