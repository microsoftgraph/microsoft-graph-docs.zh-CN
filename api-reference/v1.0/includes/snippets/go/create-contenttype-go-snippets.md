---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84a9b49d72b715a53d22b100fe6004a131369c0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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