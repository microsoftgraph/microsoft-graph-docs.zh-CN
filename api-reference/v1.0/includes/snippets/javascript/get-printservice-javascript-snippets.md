---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e3b5f10179d0d241e963083212ee1fdc483fab0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printService = await client.api('/print/services/{printServiceId}')
    .get();

```