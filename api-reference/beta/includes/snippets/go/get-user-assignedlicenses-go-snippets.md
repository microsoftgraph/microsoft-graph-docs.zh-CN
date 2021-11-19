---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4438f2340cb2f1e0a40110dbb68f958a5e28f931
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "id,mail,assignedLicenses",
    Filter: "assignedLicenses/any(u:u/skuId%20eq%20cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)",
}
options := &msgraphsdk.UsersRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Users().Get(options)


```