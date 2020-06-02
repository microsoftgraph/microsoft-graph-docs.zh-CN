---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cb85cf1ed77f103ec9225fdfd0a140a7df6b025
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests')
    .version('beta')
    .get();

```