---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc0b3790dc8f072ce16babeef61e914940ba4816
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .delete();

```