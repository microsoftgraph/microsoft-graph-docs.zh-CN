---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f105277652f6d6eeef26a3c0deb0b429f617ba6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: 'Vacation Plan'
};

await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .update(todoTaskList);

```