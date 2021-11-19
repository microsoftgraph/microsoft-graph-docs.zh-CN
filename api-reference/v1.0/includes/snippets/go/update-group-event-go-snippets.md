---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efaa763f8868e692e3747c1eabbc3031b062c9d7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101338"
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
graphClient.GroupsById(&groupId).Calendar().EventsById(&eventId).Patch(options)


```