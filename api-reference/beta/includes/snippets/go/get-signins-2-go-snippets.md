---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89976d1e37dccabbb509f5b087e9472480353c33
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095920"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SignInsRequestBuilderGetQueryParameters{
    Filter: "startsWith(appDisplayName,'Azure')",
    Top: 10,
}
options := &msgraphsdk.SignInsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AuditLogs().SignIns().Get(options)


```