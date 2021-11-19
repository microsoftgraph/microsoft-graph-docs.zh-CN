---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055a2e1b5239b9be6589cad2695e5dcea57eddee
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103857"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Filter: "mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT(groupTypes/any(s:s%20eq%20'Unified'))%20and%20membershipRuleProcessingState%20eq%20'On'",
    Count: true,
    Select: "id,membershipRule,membershipRuleProcessingState",
}
options := &msgraphsdk.GroupsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Groups().Get(options)


```