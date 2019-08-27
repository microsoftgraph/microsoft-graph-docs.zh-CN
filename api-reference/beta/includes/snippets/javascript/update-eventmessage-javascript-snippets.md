---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a89ee79e7135a324ef099d399c123b3426eb3a3a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: "true",
};

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .update(message);

```