---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 017ebcbc9488c35bb0e416a5e364f706f0e5b06e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRbacResourceNamespaceId := "unifiedRbacResourceNamespace-id"
unifiedRbacResourceActionId := "unifiedRbacResourceAction-id"
result, err := graphClient.RoleManagement().Directory().ResourceNamespacesById(&unifiedRbacResourceNamespaceId).ResourceActionsById(&unifiedRbacResourceActionId).Get(nil)


```