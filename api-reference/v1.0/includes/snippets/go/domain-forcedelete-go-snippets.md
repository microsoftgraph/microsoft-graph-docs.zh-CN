---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2da800f2e2b3d153f3ed9eb2314779067b0ea8e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
disableUserAccounts := true
requestBody.SetDisableUserAccounts(&disableUserAccounts)
options := &msgraphsdk.ForceDeleteRequestBuilderPostOptions{
    Body: requestBody,
}
domainId := "domain-id"
graphClient.DomainsById(&domainId).ForceDelete().Post(options)


```