---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6b8f03047ed5802a44546fc1ae3fa74ef44e87c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327889"
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
result, err := graphClient.Me().Profile().Languages().Post(requestBody)


```