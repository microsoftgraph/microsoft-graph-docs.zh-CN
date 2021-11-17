---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a0df70456324e143c49c8445014ba59acf117ac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
graphClient.TeamsById(&teamId).Unarchive().Post(options)


```