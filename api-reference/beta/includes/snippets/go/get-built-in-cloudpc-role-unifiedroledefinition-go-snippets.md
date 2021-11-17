---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6e49f4173ef9348a1c7e6197494ab37dee0fa4b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().CloudPC().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```