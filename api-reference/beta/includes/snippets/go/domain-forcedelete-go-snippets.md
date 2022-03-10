---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc38282f06241911952120afc7e0a06040ad482a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412164"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDisableUserAccountsRequestBody()
disableUserAccounts := true
requestBody.SetDisableUserAccounts(&disableUserAccounts)
options := &msgraphsdk.ForceDeleteRequestBuilderPostOptions{
    Body: requestBody,
}
domainId := "domain-id"
graphClient.DomainsById(&domainId).ForceDelete(domain-id).Post(options)


```