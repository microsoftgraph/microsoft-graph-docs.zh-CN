---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59d9c5bf9d9e6072f9ce99364478c9b3051be686
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let instances = await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```