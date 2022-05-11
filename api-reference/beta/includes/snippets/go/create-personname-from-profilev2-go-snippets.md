---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc8254f9e92d8c375971de6aed754ab4fa3f7537
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327888"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonName()
displayName := "Innocenty Popov"
requestBody.SetDisplayName(&displayName)
first := "Innocenty"
requestBody.SetFirst(&first)
initials := "IP"
requestBody.SetInitials(&initials)
last := "Popov"
requestBody.SetLast(&last)
languageTag := "en-US"
requestBody.SetLanguageTag(&languageTag)
requestBody.SetMaiden(nil)
result, err := graphClient.Me().Profile().Names().Post(requestBody)


```