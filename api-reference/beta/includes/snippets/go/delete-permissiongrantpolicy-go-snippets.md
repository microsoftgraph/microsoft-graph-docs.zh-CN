---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21fb7178d2421ea1b55312aa73d3c9d23b53667e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329011"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Delete()


```