---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8983c459cd5b98347ad0036a92ab3673e903edeb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092449"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.HealthOverviewsRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.HealthOverviewsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviews().Get(options)


```