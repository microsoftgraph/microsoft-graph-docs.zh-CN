---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfa1077f9ff04abd6392b2e3ffed9e7561b34fa4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPersonAnnualEvent()
type := "birthday"
requestBody.SetType(&type)
date := "1980-01-08"
requestBody.SetDate(&date)
options := &msgraphsdk.AnniversariesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Anniversaries().Post(options)


```