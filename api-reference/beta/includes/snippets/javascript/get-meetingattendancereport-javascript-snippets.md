---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f0912fd6cfae60e133423197a8956b892c962d7a57fb59b7a72b6b66d7dbfe7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let meetingAttendanceReport = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport')
    .version('beta')
    .get();

```