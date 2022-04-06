---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e019f8ff80e58eda5c28c24c8ae8f90ccb7ecc8
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DriveItemRequestBuilderGetQueryParameters{
    Expand: "children",
}
options := &msgraphsdk.DriveItemRequestBuilderGetOptions{
    Q: requestParameters,
}
driveItemId := "driveItem-id"
result, err := graphClient.Drive().ItemsById(&driveItemId).Get(options)


```