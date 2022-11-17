---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa16b76ae4cf21faca3bb8be3bbd60a06a17faab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "id,mail,assignedLicenses",
    Filter: "assignedLicenses/any(u:u/skuId%20eq%20cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```