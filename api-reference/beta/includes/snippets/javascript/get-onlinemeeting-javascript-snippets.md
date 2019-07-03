---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35f669d6d339991e5c224bf652f800faae7ac5ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/onlineMeetings/{id}')
    .version('beta')
    .get();

```