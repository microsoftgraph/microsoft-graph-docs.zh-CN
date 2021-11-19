---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d053b1f99e611185d18041692eab1174a6859e47
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085937"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Filter: "id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```