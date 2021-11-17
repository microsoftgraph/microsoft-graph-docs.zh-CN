---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfbd299c6af43de31a76c2bcd2401bab5439ab3c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007635"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.NamesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Names().Post(options)


```