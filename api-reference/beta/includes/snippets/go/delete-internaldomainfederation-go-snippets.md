---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b132129cbf8b524df16632a1df3f6a090d47a16
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327979"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Delete()


```