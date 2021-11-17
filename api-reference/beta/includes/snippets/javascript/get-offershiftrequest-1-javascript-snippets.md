---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72f18ef8f815fcae0cb46b3b2f0cbf16ceb0c67325cc11eeb541532cb9a401e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequest = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}')
    .version('beta')
    .get();

```