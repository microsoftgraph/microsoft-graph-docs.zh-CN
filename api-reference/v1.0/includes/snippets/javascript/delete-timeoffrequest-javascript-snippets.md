---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52dff184126974861db89046fc56d145a88a2df7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .delete();

```