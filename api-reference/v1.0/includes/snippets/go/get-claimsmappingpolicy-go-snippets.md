---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8440a25d08224508157cf1e715444ae3081bbefc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083123"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

claimsMappingPolicyId := "claimsMappingPolicy-id"
result, err := graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Get(options)


```