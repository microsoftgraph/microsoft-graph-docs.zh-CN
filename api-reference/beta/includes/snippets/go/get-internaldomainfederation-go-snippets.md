---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3cacf01c5899a02470ab7b5cc2830b78adbc23
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212162"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
result, err := graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Get(nil)


```