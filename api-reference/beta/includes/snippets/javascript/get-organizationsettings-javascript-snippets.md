---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a387cec8b3d0f22e3802dce74203deea9844930e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationSettings = await client.api('/organization/a9f3c90b-04fd-4504-a302-47672bbca6c8/settings')
    .version('beta')
    .get();

```