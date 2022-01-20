---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15426709c4a68d32862f165591926c362ea40979
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingAttendanceReportCollectionPage attendanceReports = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").attendanceReports()
    .buildRequest()
    .get();

```