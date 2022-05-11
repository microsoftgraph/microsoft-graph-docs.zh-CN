---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99dc1e940ffbeeeffe35606786c55633d3d0c3d7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327013"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityUserFlowAttributeAssignmentId := "identityUserFlowAttributeAssignment-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignmentsById(&identityUserFlowAttributeAssignmentId).Delete()


```