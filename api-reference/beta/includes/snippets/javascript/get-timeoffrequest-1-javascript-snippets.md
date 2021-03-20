---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09c8d51933fb601a5732d5c015c751f0a91d87c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequest = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .get();

```