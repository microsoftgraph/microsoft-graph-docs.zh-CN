---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b5c989f8c8d56b2132ec85794f08653b0e9f91
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025254"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
result, err := graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Get(options)


```