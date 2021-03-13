---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3043aca5b3ec63acea51dbb3faf4d069a7e94794
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOff = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .get();

```