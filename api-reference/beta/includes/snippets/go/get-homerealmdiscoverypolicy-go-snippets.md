---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2224b7222e01c87251baee84dbb5de5d36e52088
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086382"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
result, err := graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Get(options)


```