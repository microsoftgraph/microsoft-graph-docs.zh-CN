---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9971f2fa12690a8363f5436d05873c07cbd329ec
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083650"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Delete(options)


```