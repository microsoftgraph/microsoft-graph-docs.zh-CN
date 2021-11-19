---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 760df070af6e70add8e382395ed709320dbde588
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083414"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServiceHealthRequestBuilderGetQueryParameters{
    Expand: "issues",
}
options := &msgraphsdk.ServiceHealthRequestBuilderGetOptions{
    Q: requestParameters,
}
serviceHealthId := "serviceHealth-id"
result, err := graphClient.Admin().ServiceAnnouncement().HealthOverviewsById(&serviceHealthId).Get(options)


```