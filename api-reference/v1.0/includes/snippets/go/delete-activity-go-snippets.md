---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7db6b180275e46b92a37edcd535904d986c043b8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411621"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
result, err := graphClient.Me().ActivitiesById(&userActivityId).Delete(nil)


```