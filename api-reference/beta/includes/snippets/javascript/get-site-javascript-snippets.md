---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aadbb95e95d62ab79526e63f37972ca48109228
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783650"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let site = await client.api('/sites/{site-id}')
    .version('beta')
    .get();

```