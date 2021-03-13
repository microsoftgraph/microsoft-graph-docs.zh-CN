---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf2ca1d622053c417e3964bc05bdc32f5ce237a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let myDecisions = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions')
    .version('beta')
    .get();

```