---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4be406eba9fa955b691705d9d31e830e54307bf3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Contoso Life v2.0"
requestBody.SetDescription(&description)
displayName := "Contoso Life Renewed"
requestBody.SetDisplayName(&displayName)
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(requestBody)


```