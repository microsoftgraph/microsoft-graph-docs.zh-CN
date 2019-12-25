---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a66d7553e26833db9557b8e5bf091b6f255e39a5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/swapShiftsChangeRequests')
    .version('beta')
    .get();

```