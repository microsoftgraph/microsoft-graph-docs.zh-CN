---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3774c72326075c8689192c1d4c6cda3ea7e6d6c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/{id}')
    .get();

```