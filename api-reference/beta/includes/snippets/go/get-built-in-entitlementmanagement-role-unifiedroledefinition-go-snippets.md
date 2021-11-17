---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9877f168746970d330df03d62cceb4817ccadf0e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033506"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```