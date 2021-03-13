---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5a8eb51b1b93b98dafb7ed6228190941e3bddd0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationThread = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .get();

```