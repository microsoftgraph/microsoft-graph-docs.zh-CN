---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5594304e6b032610467d427ba579b2632bb0ce9c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326081"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewColumnDefinition()
required := true
requestBody.SetRequired(&required)
hidden := false
requestBody.SetHidden(&hidden)
propagateChanges := false
requestBody.SetPropagateChanges(&propagateChanges)
siteId := "site-id"
contentTypeId := "contentType-id"
columnDefinitionId := "columnDefinition-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).ColumnsById(&columnDefinitionId).Patch(requestBody)


```