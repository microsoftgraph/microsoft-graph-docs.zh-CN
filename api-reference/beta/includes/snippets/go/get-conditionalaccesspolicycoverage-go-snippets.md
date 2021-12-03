---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c174975706b123c22b98056b03ca8f4d1d3660c3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyCoverageId := "conditionalAccessPolicyCoverage-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ConditionalAccessPolicyCoveragesById(&conditionalAccessPolicyCoverageId).Get(nil)


```