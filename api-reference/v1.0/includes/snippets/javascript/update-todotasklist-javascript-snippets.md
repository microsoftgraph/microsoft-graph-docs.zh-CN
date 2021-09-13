---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16747c53ee959edbb0ae4a9761127cbeb56b1d42d546283b52f0279aafda0d1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219621"
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