---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac8f929907a53d25a9c82c88ec51c1a02ecc1682
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022370"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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