---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d7a51c984242fc2d657eed62f7531d21529ce4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tiIndicators = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```