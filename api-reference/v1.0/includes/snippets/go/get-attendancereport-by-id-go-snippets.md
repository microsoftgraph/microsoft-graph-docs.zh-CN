---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba131ec2df9242a1698de07ff65a828b5e299dca
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326838"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MeetingAttendanceReportRequestBuilderGetQueryParameters{
    Expand: "attendanceRecords",
}
options := &msgraphsdk.MeetingAttendanceReportRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onlineMeetingId := "onlineMeeting-id"
meetingAttendanceReportId := "meetingAttendanceReport-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).AttendanceReportsById(&meetingAttendanceReportId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```