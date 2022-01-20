---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02569295ceeb3e2d7017ee1e9aab7168a887212c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101788"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onlineMeetingId := "onlineMeeting-id"
meetingAttendanceReportId := "meetingAttendanceReport-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).AttendanceReportsById(&meetingAttendanceReportId).AttendanceRecords().Get(nil)


```