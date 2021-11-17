---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50ac1101cf9826549a6760fd0c93650fe64f4191
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015721"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UsageRightsRequestBuilderGetQueryParameters{
    Filter: "state%20in%20('active',%20'suspended')%20and%20serviceIdentifier%20in%20('ABCD')",
}
options := &msgraphsdk.UsageRightsRequestBuilderGetOptions{
    Q: requestParameters,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).UsageRights().Get(options)


```