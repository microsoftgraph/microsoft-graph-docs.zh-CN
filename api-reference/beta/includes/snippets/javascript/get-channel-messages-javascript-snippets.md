---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72ab69532a4094bc165ec202d28860224ca55bed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages')
    .version('beta')
    .get();

```