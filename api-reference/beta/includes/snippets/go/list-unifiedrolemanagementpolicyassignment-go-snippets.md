---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edaf8e598d0e4a7543ae873cf1f1d15fe9547f10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019640"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().RoleManagementPolicyAssignments().Get(options)


```