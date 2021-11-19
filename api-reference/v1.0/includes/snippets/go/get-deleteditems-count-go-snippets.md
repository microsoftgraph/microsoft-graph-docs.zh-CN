---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecc84137d1a147b125c2478631c8bc23d44f9c9e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    OrderBy: "deletedDateTime%20asc",
    Select: "id,DisplayName,deletedDateTime",
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