---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f08f8a58a8654517904f1c3a2a8893f0504f6427
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086676"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDriveItem()
name := "Just some files"
requestBody.SetName(&name)
bundle := msgraphsdk.NewBundle()
requestBody.SetBundle(bundle)
requestBody.SetChildren( []DriveItem {
    msgraphsdk.NewDriveItem(),
    SetAdditionalData(map[string]interface{}{
        "id": "1234asdf",
    }
    msgraphsdk.NewDriveItem(),
    SetAdditionalData(map[string]interface{}{
        "id": "1234qwerty",
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