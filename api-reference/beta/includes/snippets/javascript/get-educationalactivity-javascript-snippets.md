---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec5f85a49a62e73439f9d848709eb4be5b63f05b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationalActivity = await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .get();

```