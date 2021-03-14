---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6b7778d0f5b9153891736441c81341f4649901f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shift = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .get();

```