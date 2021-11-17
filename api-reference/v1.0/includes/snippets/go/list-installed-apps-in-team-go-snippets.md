---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 676db82b46d2e2f6cd968e6a099fe71c48a13e3b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016135"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).InstalledApps().Get(options)


```