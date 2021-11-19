---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33afb6be7c4476680e1bfb6ea1e03a529e5f01f6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SitesRequestBuilderGetQueryParameters{
    Select: "siteCollection,webUrl",
    Filter: "siteCollection/root%20ne%20null",
}
options := &msgraphsdk.SitesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Sites().Get(options)


```