---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba9b7cd787c9a4f156a7135f7ab155bbba060081
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411818"
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
result, err := graphClient.Drive().ItemsById(&driveItemId).Patch(options)


```