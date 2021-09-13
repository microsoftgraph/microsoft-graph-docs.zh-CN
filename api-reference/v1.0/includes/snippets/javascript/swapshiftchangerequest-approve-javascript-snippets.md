---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63602eac1147a577b7de4ea069dfa814e920251ce8e6a7a456bb59eb1950f90b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .post(approve);

```