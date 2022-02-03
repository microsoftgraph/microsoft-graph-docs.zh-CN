---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c16910b292d919cc17bfb1141cf07a9b74633547
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CloudPCRequestBuilderGetQueryParameters{
    Select: "id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult",
}
options := &msgraphsdk.CloudPCRequestBuilderGetOptions{
    Q: requestParameters,
}
cloudPCId := "cloudPC-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).Get(options)


```