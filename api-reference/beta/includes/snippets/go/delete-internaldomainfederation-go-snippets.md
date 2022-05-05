---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ad443f4cd9f33895e0564d23bf83fa85b98f6f5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Delete(nil)


```