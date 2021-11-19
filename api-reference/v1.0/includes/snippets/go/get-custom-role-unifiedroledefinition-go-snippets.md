---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d929e14d297ed3377581cb073f2585607cc9b2e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```