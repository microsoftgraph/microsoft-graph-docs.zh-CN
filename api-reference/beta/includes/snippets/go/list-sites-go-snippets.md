---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b2d359714be7d4bca5d6144d04fa2e571848a13
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033725"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.SitesRequestBuilderGetQueryParameters{
    Select: "siteCollection,webUrl",
    Filter: "siteCollection/root%20ne%20null",
}
options := &msgraphsdk.SitesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Sites().Get(options)


```