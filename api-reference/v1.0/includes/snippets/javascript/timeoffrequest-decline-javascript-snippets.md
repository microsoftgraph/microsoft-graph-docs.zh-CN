---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d35cfc0432fbaa2bc18a48a3230b00981b2787d2922c92a8c1f6ee8309cec9ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline')
    .post(decline);

```