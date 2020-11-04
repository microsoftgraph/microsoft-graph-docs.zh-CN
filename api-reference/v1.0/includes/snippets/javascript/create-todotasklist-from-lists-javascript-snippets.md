---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65612c3c8eae41d2dd0774a8754be5c2a519f3fa
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Travel items"
};

let res = await client.api('/me/todo/lists')
    .post(todoTaskList);

```