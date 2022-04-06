---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ce54bc700503a6448e33274472f74b0989a4458
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758054"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDriveItem()
name := "Shared legal agreements"
requestBody.SetName(&name)
options := &msgraphsdk.DriveItemRequestBuilderPatchOptions{
    Body: requestBody,
}
driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Patch(options)


```