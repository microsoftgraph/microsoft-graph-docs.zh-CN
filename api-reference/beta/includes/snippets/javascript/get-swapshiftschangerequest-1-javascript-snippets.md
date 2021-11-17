---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d790b895bcda7e5e25b32f411006239c16e78b399c5cf7fe68dcddf07208071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let swapShiftsChangeRequest = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}')
    .version('beta')
    .get();

```