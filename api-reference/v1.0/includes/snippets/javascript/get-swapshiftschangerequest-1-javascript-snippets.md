---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96222736999ee99f41a30d22540de5e40e6a5eb7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let swapShiftsChangeRequest = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}')
    .get();

```