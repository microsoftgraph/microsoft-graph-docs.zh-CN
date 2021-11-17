---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8830998793af319746b105b58ae574ef0634aa76
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.GroupsById(&groupId).Calendar().EventsById(&eventId).Patch(options)


```