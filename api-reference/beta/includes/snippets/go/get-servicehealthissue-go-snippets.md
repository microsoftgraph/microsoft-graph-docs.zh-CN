---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42b5ef9f478e5a3e03439f95c324d6c9aa686336
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031905"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

serviceHealthIssueId := "serviceHealthIssue-id"
result, err := graphClient.Admin().ServiceAnnouncement().IssuesById(&serviceHealthIssueId).Get(options)


```