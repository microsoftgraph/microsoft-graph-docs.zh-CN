---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ce54bc700503a6448e33274472f74b0989a4458
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086938"
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