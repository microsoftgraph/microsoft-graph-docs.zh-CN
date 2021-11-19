---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fac3408a2e77f5270d8a9f5e8b40bd9cc514c5c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101973"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
result, err := graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Get(options)


```