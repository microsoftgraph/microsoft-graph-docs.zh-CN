---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db063bfb28ecf6ec2d4f7ab0b6ff0df26c6961fc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098424"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    StartDateTime: "2020-01-01T19:00:00-08:00",
    EndDateTime: "2020-01-02T19:00:00-08:00",
}
options := &msgraphsdk.CalendarViewRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().CalendarView().Get(options)


```