---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed56d50f60cd5b4a1f7b18811cf00b7a9a42f70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: 'Cancelling for this week due to all hands'
};

await client.api('/me/events/{id}/cancel')
    .post(cancel);

```