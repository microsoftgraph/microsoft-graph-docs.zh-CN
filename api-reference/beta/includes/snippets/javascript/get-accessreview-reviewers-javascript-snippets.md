---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56ca7ff944382c74a848b2e6a0869c05691189d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewers = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .get();

```