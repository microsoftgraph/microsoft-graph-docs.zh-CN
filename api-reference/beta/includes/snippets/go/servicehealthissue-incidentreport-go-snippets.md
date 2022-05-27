---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b86bb7f7d4ff596715a4fe1f86395c69f72ee2b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719278"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthIssueId := "serviceHealthIssue-id"
graphClient.Admin().ServiceAnnouncement().IssuesById(&serviceHealthIssueId).IncidentReport()(serviceHealthIssue-id).Get()


```