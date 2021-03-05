---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a6927b8db95e871f99f403c68342d7e7b11965b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "message-value"
};

let res = await client.api('/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve')
    .post(approve);

```