---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9426894e92a8d3048301fb62f62fa26546a0fa75
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805602"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/users/{id}/outlook/tasks/{id}/attachments')
    .version('beta')
    .get();

```