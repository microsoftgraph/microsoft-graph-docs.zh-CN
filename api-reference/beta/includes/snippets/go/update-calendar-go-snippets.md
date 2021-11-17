---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ab0337df8706af29a8a08661ea9d08957143e23
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015705"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCalendar()
name := "Social events"
requestBody.SetName(&name)
options := &msgraphsdk.CalendarRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Calendar().Patch(options)


```