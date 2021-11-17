---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30b97a4aa0b085ce02ac620e2f5988b97ad8699b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032808"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
options := &msgraphsdk.TermStoreRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
graphClient.SitesById(&siteId).TermStore().Patch(options)


```