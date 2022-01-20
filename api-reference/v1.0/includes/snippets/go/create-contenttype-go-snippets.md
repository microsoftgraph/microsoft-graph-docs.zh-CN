---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc3024def0c24a4bbbd49f1253d0625e7d597a89
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110612"
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
options := &msgraphsdk.ContentTypesRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).ContentTypes().Post(options)


```