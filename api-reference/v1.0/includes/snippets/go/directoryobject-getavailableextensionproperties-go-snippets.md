---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e46d379c2f49350063d9a9caa030109694bf755f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973997"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
isSyncedFromOnPremises := "Boolean"
requestBody.SetIsSyncedFromOnPremises(&isSyncedFromOnPremises)
options := &msgraphsdk.GetAvailableExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryObjects().GetAvailableExtensionProperties().Post(options)


```