---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ac405d73998a77d759ac8fd3d47ca1fb39c36db
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
contentTypeId := "String"
requestBody.SetContentTypeId(&contentTypeId)
options := &msgraphsdk.AddCopyFromContentTypeHubRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopyFromContentTypeHub().Post(options)


```