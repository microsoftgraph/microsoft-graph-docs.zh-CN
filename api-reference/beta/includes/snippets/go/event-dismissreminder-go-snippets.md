---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a95675562194c64b09882017fadf570ed9398f2e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088394"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

eventId := "event-id"
graphClient.Me().EventsById(&eventId).DismissReminder().Post(options)


```