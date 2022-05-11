---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08bb787fd0d68cf28d0d37defbcedb29adcc9e1d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327294"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttributeSet()
description := "Attributes for engineering team"
requestBody.SetDescription(&description)
maxAttributesPerSet := int32(20)
requestBody.SetMaxAttributesPerSet(&maxAttributesPerSet)
attributeSetId := "attributeSet-id"
graphClient.Directory().AttributeSetsById(&attributeSetId).Patch(requestBody)


```