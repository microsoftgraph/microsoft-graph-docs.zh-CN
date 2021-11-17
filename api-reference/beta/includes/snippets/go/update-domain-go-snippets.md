---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d977a974984bc1f9eb4f0c460c720502e91b9f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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