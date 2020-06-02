---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e66d56861aa980b94530fd8a8e1e87475437249
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "40867759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .get();

```