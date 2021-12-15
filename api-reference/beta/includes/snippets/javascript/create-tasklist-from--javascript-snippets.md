---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3738b6ce4a45a057b860b275da8fd1c14bdea095
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const lists = {
    displayName: 'Shopping list'
};

await client.api('/me/tasks/lists')
    .version('beta')
    .post(lists);

```