---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca7500c5fbbcf3e34b341c2f850398e3793cb61
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttendanceRecordCollectionPage attendanceRecords = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").attendanceReports("c9b6db1c-d5eb-427d-a5c0-20088d9b22d7").attendanceRecords()
    .buildRequest()
    .get();

```