---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cd48fdb77f905cc25f5ab4eb6943377c9a1f320
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028927"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.InstalledAppsRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition",
}
options := &msgraphsdk.InstalledAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Teamwork().InstalledApps().Get(options)


```