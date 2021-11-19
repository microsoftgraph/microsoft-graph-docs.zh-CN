---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f14288c1df66c9b5d9727d9fb1ee8a8e56810ae2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
options := &msgraphsdk.TermStoreRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
graphClient.SitesById(&siteId).TermStore().Patch(options)


```