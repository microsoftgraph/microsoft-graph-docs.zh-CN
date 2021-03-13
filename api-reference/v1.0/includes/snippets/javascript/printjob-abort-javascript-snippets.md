---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7370199324c479ca3da9a81827602e89ad50871c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771398"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const abort = {
  reason: 'String'
};

await client.api('/print/printers/{printerId}/jobs/{printJobId}/abort')
    .post(abort);

```