---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9b6217c6ede2cec3b9d15fe8ebf5c5c065d28b1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326681"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
result, err := graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Get()


```