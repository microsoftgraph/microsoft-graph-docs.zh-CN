---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d4ebd9e51531d4e79959c73d4519267826359f7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447877"
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
    .version('beta')
    .post(approve);

```