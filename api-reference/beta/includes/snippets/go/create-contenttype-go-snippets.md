---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5edd83248e265fc2be80446dec857ebf7fa5df0b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328830"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentType()
name := "docSet"
requestBody.SetName(&name)
description := "custom docset"
requestBody.SetDescription(&description)
base := msgraphsdk.NewContentType()
requestBody.SetBase(base)
name := "Document Set"
base.SetName(&name)
id := "0x0120D520"
base.SetId(&id)
group := "Document Set Content Types"
requestBody.SetGroup(&group)
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).ContentTypes().Post(requestBody)


```