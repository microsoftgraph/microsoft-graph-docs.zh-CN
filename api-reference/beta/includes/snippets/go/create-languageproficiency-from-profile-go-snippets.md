---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aa271aa4b47ace7c695da71c3efb2a877a6c67c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewLanguageProficiency()
displayName := "Norwegian Bokmål"
requestBody.SetDisplayName(&displayName)
tag := "nb-NO"
requestBody.SetTag(&tag)
spoken := "nativeOrBilingual"
requestBody.SetSpoken(&spoken)
written := "nativeOrBilingual"
requestBody.SetWritten(&written)
reading := "nativeOrBilingual"
requestBody.SetReading(&reading)
options := &msgraphsdk.LanguagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Languages().Post(options)


```