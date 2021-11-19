---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9be1a56a247b558b29c3164f19dd9ff6eb9b3229
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086379"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onlineMeetingId := "onlineMeeting-id"
meetingRegistrationQuestionId := "meetingRegistrationQuestion-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Get(options)


```