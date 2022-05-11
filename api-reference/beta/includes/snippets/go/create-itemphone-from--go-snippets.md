---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5f36d144f9a7a788dc194ef7c4cdee002537ad6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326037"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPhone()
displayName := "Car Phone"
requestBody.SetDisplayName(&displayName)
number := "+7 499 342 22 13"
requestBody.SetNumber(&number)
result, err := graphClient.Me().Profile().Phones().Post(requestBody)


```