---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30604ea6b1f35ac0b7f0da3fbe1da6ff53cda826
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976181"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
graphClient.TeamsById(&teamId).CompleteMigration().Post(options)


```