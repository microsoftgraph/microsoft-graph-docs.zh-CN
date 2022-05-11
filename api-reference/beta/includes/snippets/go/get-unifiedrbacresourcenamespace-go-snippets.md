---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb076f5934f6da7991456c578bac561865d172c3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRbacResourceNamespaceId := "unifiedRbacResourceNamespace-id"
result, err := graphClient.RoleManagement().Directory().ResourceNamespacesById(&unifiedRbacResourceNamespaceId).Get()


```