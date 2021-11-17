---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 058551508d8a0758b21d87b8992a7aa38a7facf5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012668"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewDriveItem()
name := "Shared legal agreements"
requestBody.SetName(&name)
options := &msgraphsdk.DriveItemRequestBuilderPatchOptions{
    Body: requestBody,
}
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Patch(options)


```