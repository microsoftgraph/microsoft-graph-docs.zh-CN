---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a756b9ee46292ba0dfb3239f3e4570a299d4bc3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationUserId := "educationUser-id"
graphClient.Education().ClassesById(&educationClassId).MembersById(&educationUserId).Delete()


```