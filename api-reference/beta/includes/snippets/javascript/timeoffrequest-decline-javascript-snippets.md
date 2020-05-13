---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7cfe46666024d7affddd2c0b6c0e20836f98638
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline')
    .version('beta')
    .post(decline);

```