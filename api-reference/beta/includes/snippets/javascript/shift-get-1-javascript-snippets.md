---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d644eef47310cf0e6d42c2ccf8aede97b90a647
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shift = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .get();

```