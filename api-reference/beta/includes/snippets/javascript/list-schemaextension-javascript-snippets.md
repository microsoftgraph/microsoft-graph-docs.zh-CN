---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51747738f0f9a60277400cf1dc84c545f6b9dc5c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .select('ext55gb1l09_msLearnCourses')
    .get();

```