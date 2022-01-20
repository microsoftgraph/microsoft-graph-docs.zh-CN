---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5f2b8a7e1544a08d885425af86ee125a2e97e05
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let meetingAttendanceReport = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')
    .expand('attendanceRecords')
    .get();

```