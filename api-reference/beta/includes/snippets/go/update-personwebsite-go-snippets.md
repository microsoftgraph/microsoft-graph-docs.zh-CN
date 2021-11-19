---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07ff9c03651e881688c3f61f4c0d177260570d3c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonWebsite()
description := "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
requestBody.SetDescription(&description)
options := &msgraphsdk.PersonWebsiteRequestBuilderPatchOptions{
    Body: requestBody,
}
personWebsiteId := "personWebsite-id"
graphClient.Me().Profile().WebsitesById(&personWebsiteId).Patch(options)


```