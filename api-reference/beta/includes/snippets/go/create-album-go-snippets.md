---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3002b2db37f4fe7fb94ba2d99b24756cd3978c10
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDriveItem()
name := "My Day at the Beach"
requestBody.SetName(&name)
bundle := msgraphsdk.NewBundle()
requestBody.SetBundle(bundle)
album := msgraphsdk.NewAlbum()
bundle.SetAlbum(album)
requestBody.SetChildren( []DriveItem {
    msgraphsdk.NewDriveItem(),
    SetAdditionalData(map[string]interface{}{
        "id": "1234asdf",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@microsoft.graph.conflictBehavior": "rename",
}
options := &msgraphsdk.BundlesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Drive().Bundles().Post(options)


```