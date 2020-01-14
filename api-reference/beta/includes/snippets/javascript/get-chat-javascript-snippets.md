---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fac72fb98be0a82a0e2480ad3efd5d76ba79c5e
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/chats/{id}')
    .version('beta')
    .get();

```