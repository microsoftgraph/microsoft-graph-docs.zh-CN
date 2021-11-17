---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d19b5ef5ddc44b31e38d4e473373d0c29f9e079
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974654"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'876df28f-2e78-423b-94a5-44181bd0e225'",
    Expand: "appDefinitions",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```