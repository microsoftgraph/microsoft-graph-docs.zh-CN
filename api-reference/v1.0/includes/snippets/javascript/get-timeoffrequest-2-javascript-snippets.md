---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68f33d2a22c6d1f22eb23e8c06060137135e0fca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequests = await client.api('/teams/{teamId}/schedule/timeOffRequests')
    .get();

```