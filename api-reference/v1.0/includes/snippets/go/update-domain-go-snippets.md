---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af5a27c003a32bc867ad502c70991ee52e185e45
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098983"
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
graphClient.DomainsById(&domainId).Patch(options)


```