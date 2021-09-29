---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b61a312b316854bf130ba659f7ae7208ca6a388
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996428"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingAttendanceReport meetingAttendanceReport = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy").meetingAttendanceReport()
    .buildRequest()
    .get();

```