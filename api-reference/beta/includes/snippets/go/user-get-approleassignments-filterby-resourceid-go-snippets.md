---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78df5d1e383a7f5ed6c619c90b914fa54d4c6cd5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088847"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "resourceId%20eq%208e881353-1735-45af-af21-ee1344582a4d",
}
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().Get(options)


```