---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edec52c7aae722c278f9cdfc02dc1d9179560e7f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411713"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
result, err := graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Delete(nil)


```