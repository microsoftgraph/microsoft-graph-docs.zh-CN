---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6187f08e20bcc001f9dba1b2b99f18f71a7c9b7b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
teamworkTagMemberId := "teamworkTagMember-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).MembersById(&teamworkTagMemberId).Delete(options)


```