---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47dfda0b992cb5c4cb1527da2cd80a7f3a97382d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
    ext55gb1l09_msLearnCourses: {
        courseType: 'Admin'
    }
};

await client.api('/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e')
    .version('beta')
    .update(user);

```