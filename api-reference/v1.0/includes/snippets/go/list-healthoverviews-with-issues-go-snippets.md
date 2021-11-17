---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e54147a8e679bdcaa1911baeb462f15150f19f6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021273"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.HealthOverviewsRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.HealthOverviewsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().Get(options)


```