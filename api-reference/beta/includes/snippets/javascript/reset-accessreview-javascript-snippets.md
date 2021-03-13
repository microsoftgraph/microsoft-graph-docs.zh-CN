---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b5ba291010980c3961f2126406b6e140216d569
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions')
    .version('beta')
    .post();

```