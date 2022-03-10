---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3f0ae0da99299e76b275cbc019c933dfed5e307
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttributeSet()
description := "Attributes for engineering team"
requestBody.SetDescription(&description)
maxAttributesPerSet := int32(20)
requestBody.SetMaxAttributesPerSet(&maxAttributesPerSet)
options := &msgraphsdk.AttributeSetRequestBuilderPatchOptions{
    Body: requestBody,
}
attributeSetId := "attributeSet-id"
result, err := graphClient.Directory().AttributeSetsById(&attributeSetId).Patch(options)


```