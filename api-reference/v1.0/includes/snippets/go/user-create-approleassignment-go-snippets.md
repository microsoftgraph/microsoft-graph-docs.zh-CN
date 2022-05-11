---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2625eb32572db4bcf957454ddcc3caf6bec77c2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppRoleAssignment()
principalId := "cde330e5-2150-4c11-9c5b-14bfdc948c79"
requestBody.SetPrincipalId(&principalId)
resourceId := "8e881353-1735-45af-af21-ee1344582a4d"
requestBody.SetResourceId(&resourceId)
appRoleId := "00000000-0000-0000-0000-000000000000"
requestBody.SetAppRoleId(&appRoleId)
userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().Post(requestBody)


```