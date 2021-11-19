---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea107dc5bdcb4b62c5b98891bd2b86aa385abbe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Filter: "externalId%20eq%20'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().Get(options)


```