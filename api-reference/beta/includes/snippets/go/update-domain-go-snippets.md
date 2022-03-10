---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d36a42d020c7af927806259c2bdc88a046356718
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDomain()
isDefault := true
requestBody.SetIsDefault(&isDefault)
requestBody.SetSupportedServices( []String {
    "Email",
    "OfficeCommunicationsOnline",
}
options := &msgraphsdk.DomainRequestBuilderPatchOptions{
    Body: requestBody,
}
domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).Patch(options)


```