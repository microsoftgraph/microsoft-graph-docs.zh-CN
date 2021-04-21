---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db526b434c11aeb4d2dd4feacfb466152097c02c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920410"
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