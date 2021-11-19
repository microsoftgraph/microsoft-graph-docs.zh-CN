---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74ce595dc5d0a588d980a1f68c67dccb942cd4b5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096908"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().RoleManagementPolicyAssignments().Get(options)


```