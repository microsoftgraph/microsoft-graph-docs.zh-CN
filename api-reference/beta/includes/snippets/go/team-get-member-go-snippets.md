---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9835703709626c94da10a555b243fd04a497f0e8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).MembersById(&conversationMemberId).Get(options)


```