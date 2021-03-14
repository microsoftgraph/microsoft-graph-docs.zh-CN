---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3214f7328dfeb797e9c61c2505b1733d5995dfb1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/devices/{id}/memberOf')
    .get();

```