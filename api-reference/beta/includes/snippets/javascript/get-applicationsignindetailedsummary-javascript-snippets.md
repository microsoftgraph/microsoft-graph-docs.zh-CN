---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a7f8d0d20a8fa15472ccabfa7de965661bd4430
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationSignInDetailedSummary = await client.api('/reports/applicationSignInDetailedSummary/{id}')
    .version('beta')
    .get();

```