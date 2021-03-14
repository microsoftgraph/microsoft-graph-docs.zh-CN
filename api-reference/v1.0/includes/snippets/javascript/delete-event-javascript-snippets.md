---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2993a6742caef76d311c524d2563c1dca4a82abf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/events/{id}')
    .delete();

```