---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8263b8bde1467916ed40beab7b090656d1d9be5e40c471f8d72b78831834b73b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105307"
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
    .post(todoTaskList);

```