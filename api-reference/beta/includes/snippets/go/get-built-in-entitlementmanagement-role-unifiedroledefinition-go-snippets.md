---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cf1c103cee8a92ab82be361ef850be01a16cd7b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091790"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```