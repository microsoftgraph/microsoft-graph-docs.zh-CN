---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93e384b44e5fdc347e68d26094ea1b49dfac781d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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