---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 462b9ed8ca976c5f931942080f8b195066d01563
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008210"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DriveItemRequestBuilderGetQueryParameters{
    Expand: "children",
}
options := &msgraphsdk.DriveItemRequestBuilderGetOptions{
    Q: requestParameters,
}
driveItemId := "driveItem-id"
result, err := graphClient.Drive().ItemsById(&driveItemId).Get(options)


```