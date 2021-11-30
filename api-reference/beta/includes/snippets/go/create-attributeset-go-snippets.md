---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14eb8406d5b385aec91ef97a1e820f00141f22c
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226489"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttributeSet()
id := "Engineering"
requestBody.SetId(&id)
description := "Attributes for engineering team"
requestBody.SetDescription(&description)
maxAttributesPerSet := int32(25)
requestBody.SetMaxAttributesPerSet(&maxAttributesPerSet)
options := &msgraphsdk.AttributeSetsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().AttributeSets().Post(options)


```