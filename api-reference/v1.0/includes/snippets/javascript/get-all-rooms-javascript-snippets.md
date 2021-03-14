---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad37c15337aeae503b6470848bdf5272f77c76f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let room = await client.api('/places/microsoft.graph.room')
    .get();

```