---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ec96b0ed16577276f75bac830998e9c1f290843
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
onlineMeetingId := "onlineMeeting-id"
meetingRegistrantId := "meetingRegistrant-id"
graphClient.UsersById(&userId).OnlineMeetingsById(&onlineMeetingId).Registration().RegistrantsById(&meetingRegistrantId).Delete(options)


```