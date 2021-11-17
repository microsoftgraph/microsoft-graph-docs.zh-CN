---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d283fa6f75032f9cfc6b49f2fbae19fa6f9b944
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

claimsMappingPolicyId := "claimsMappingPolicy-id"
result, err := graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Get(options)


```