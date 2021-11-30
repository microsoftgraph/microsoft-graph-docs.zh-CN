---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15426709c4a68d32862f165591926c362ea40979
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225326"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingAttendanceReportCollectionPage attendanceReports = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").attendanceReports()
    .buildRequest()
    .get();

```