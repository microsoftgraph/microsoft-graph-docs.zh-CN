---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1efcee95b86b1c88a948a78e45ae86829c04ef56
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991064"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Expand: "appDefinitions($expand=bot)",
    Filter: "appDefinitions/any(a:a/bot%20ne%20null)",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```