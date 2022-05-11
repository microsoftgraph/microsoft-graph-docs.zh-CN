---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77b48f09cc249e23cd2d148adeac56205c352433
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327911"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDisableUserAccountsRequestBody()
disableUserAccounts := true
requestBody.SetDisableUserAccounts(&disableUserAccounts)
domainId := "domain-id"
graphClient.DomainsById(&domainId).ForceDelete(domain-id).Post(requestBody)


```