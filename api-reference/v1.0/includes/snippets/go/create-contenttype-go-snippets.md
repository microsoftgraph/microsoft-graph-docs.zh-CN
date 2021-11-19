---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5639d4a64d32630c943528882a282afbb9c7b777
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090391"
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
base.SetAdditionalData(map[string]interface{}{
    "name": "Document Set",
    "id": "0x0120D520",
}
group := "Document Set Content Types"
requestBody.SetGroup(&group)
options := &msgraphsdk.ContentTypesRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).ContentTypes().Post(options)


```