---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cda9495968d04438d0d960672c9e6a3fda2313d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).Delete(nil)


```