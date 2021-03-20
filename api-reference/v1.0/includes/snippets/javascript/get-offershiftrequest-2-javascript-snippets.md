---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c515af3d42adf48f8b5b433c54dfda3f367444ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequests = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .get();

```