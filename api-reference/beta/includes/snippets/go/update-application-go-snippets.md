---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49e1b7e5a62bb3f9b4e72a85cdbfa9e45ae715d2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326401"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewApplication()
displayName := "New display name"
requestBody.SetDisplayName(&displayName)
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Patch(requestBody)


```