---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b7349f5f9050979a55456cef49fe74b5a3f262f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{printerId}/jobs/{printJobId}/cancel')
    .post();

```