---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6f740140dfdc2845e564c9a5138b91f770da553
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412572"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Delete(nil)


```