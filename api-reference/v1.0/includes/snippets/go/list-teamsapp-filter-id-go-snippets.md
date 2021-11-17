---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91e4668310619f1744affdb362146db9ebfcc49c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```