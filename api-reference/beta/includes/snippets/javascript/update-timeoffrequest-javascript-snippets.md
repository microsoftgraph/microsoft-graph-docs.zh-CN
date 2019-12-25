---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2d6d8f0d553c7fad6c2a9cb1f93fb28faca27c3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffRequests = {
  startDateTime: "datetime-value",
  endDateTime: "datetime-value",
  timeOffReasonId: "timeOffReasonId-value"
};

let res = await client.api('/teams/{id}/schedule/timeOffRequests')
    .version('beta')
    .update(timeOffRequests);

```