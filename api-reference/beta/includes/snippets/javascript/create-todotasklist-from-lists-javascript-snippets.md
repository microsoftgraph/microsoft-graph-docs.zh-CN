---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da9a341a5d56b2b1be98ac5b8dcac0eeae891da9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777945"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: 'Travel items'
};

await client.api('/me/todo/lists')
    .version('beta')
    .post(todoTaskList);

```