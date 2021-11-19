---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc71e0471685e03f81d040c382112b4bb207c43c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100045"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Delete(options)


```