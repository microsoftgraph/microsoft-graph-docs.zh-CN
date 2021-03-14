---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ecd38fc6a8a89f6cec89d3518c8478adb3c7db3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let orgContact = await client.api('/contacts/{id}')
    .get();

```