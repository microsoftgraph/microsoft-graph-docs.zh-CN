---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec123462b78f85253a4f10841a2b5dd2180b0234
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104087"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityUserFlowAttributeAssignmentId := "identityUserFlowAttributeAssignment-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignmentsById(&identityUserFlowAttributeAssignmentId).Get(options)


```