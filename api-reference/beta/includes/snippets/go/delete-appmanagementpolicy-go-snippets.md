---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29f9a4bbdca5266f2e0d9fdb66b40c5a26b1c5d8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411848"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

appManagementPolicyId := "appManagementPolicy-id"
result, err := graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).Delete(nil)


```