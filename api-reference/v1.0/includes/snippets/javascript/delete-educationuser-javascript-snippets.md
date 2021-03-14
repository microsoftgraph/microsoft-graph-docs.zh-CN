---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b3152b511c18d9cd439bed58a75b7b04d49045
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/users/{user-id}')
    .delete();

```