---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8178c317f3c0ad55286cf0bd85bf260cd48d9520
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082408"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsageRightsRequestBuilderGetQueryParameters{
    Filter: "state%20in%20('active',%20'suspended')%20and%20serviceIdentifier%20in%20('ABCD')",
}
options := &msgraphsdk.UsageRightsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).UsageRights().Get(options)


```