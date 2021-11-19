---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e019f8ff80e58eda5c28c24c8ae8f90ccb7ecc8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093670"
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