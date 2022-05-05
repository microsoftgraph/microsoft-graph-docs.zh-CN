---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d96f89fb1fe5f532e00ebd63bb70bcdcae83a36
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204241"
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
    .update(user);

```