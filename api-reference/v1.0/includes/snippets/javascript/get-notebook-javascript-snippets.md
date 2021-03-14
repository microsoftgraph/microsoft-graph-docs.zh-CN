---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe42c9ae9ffd06c17f65bb9705df95742cc7339f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebook = await client.api('/me/onenote/notebooks/{id}')
    .get();

```