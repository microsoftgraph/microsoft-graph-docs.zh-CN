---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a35a9e6bba972c52dc18fb8b1094d436a276f3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/mentions/{id}')
    .version('beta')
    .delete();

```