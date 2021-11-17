---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f5cddc401d008d3192265c5423002a14062eb2d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "deletedDateTime%20asc",
    Select: "id,displayName,deletedDateTime",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DirectoryObjectRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
directoryObjectId := "directoryObject-id"
result, err := graphClient.Directory().DeletedItemsById(&directoryObjectId).Get(options)


```