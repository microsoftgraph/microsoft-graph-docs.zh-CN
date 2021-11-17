---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3c7dc4b2088383d1ae62881df6f674e7a018ebe
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974773"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
conversationMemberId := "conversationMember-id"
graphClient.TeamsById(&teamId).MembersById(&conversationMemberId).Delete(options)


```