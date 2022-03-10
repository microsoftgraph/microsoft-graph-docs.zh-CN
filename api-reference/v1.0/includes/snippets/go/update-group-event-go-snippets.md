---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 341bb7bfd8d0bfec4f401e47a2ca185d1c4d9ae2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEvent()
location := msgraphsdk.NewLocation()
requestBody.SetLocation(location)
displayName := "Conf Room 2"
location.SetDisplayName(&displayName)
options := &msgraphsdk.EventRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
eventId := "event-id"
result, err := graphClient.GroupsById(&groupId).Calendar().EventsById(&eventId).Patch(options)


```