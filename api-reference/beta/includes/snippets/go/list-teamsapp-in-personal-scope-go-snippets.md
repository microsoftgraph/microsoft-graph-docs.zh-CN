---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11f081dbc153babe4ba8cb72c01ecf96864b259f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Expand: "appDefinitions($select=id,displayName,allowedInstallationScopes)",
    Filter: "appDefinitions/any(a:a/allowedInstallationScopes%20has%20'personal')",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```