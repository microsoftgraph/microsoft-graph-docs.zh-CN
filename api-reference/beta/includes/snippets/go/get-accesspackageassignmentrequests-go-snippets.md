---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cfbdfe511b8c46677c94b2925bf794363d5907b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098562"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters{
    Expand: "requestor($expand=connectedOrganization)",
    Filter: "(requestState%20eq%20'PendingApproval')",
}
options := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().Get(options)


```