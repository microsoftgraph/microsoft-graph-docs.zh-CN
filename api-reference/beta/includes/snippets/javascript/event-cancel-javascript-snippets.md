---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 173f67e109d9e8cf81ebdf06f3d22aaf2bff5efc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: "Cancelling for this week due to all hands"
};

let res = await client.api('/me/events/{id}/cancel')
    .version('beta')
    .post(cancel);

```