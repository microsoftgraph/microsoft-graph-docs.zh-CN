---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3b4e7894dc7a3108c6edbf8757a2e260cd79642
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c"
};

let res = await client.api('/app/calls/{id}/subscribeToTone')
    .version('beta')
    .post(subscribeToToneOperation);

```