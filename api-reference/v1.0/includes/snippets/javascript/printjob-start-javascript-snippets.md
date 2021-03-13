---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ae9ea08ac62ecfb83c5476771e227148efa91b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/jobs/{printJobId}/start')
    .post();

```