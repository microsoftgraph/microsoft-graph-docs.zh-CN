---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e8225f4e113dbca54ce60f4b0669daf76813075
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Social events"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Calendar().Patch(options)


```