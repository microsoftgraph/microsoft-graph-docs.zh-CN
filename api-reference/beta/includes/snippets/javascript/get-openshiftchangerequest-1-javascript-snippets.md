---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 142f0f4fc9d6a5afe7f337965351ef7b68eebac8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequest = await client.api('/teams/{id}/schedule/openShiftChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09')
    .version('beta')
    .get();

```