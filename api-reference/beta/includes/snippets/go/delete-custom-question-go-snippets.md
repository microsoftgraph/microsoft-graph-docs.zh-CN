---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60309469256c03cd8edabc8c2eae76cae4d470b5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327905"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onlineMeetingId := "onlineMeeting-id"
meetingRegistrationQuestionId := "meetingRegistrationQuestion-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().CustomQuestionsById(&meetingRegistrationQuestionId).Delete()


```