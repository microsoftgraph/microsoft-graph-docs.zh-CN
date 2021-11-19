---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18f439c2be37652150b86e3fc6e8f9e693b67f67
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093061"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).AttendeeReport().Get(options)


```