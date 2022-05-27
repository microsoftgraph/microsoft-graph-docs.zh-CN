---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 677057778f728c96c3873ab6f185d3f70845e12d
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewReferenceUpdateSchema()
@odata.id := "https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
requestBody.Set@odata.id(&@odata.id)
userId := "user-id"
graphClient.UsersById(&userId).Manager().$ref().Put(requestBody)


```