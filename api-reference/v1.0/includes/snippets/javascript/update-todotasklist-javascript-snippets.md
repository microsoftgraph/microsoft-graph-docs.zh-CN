---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38c13ed52551bf44b26e17bdd0bccfc4b948b3d9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTaskList = {
  displayName: "Vacation Plan"
};

let res = await client.api('/me/todo/lists/AAMkADIyAAAhrbPWAAA=')
    .update(todoTaskList);

```