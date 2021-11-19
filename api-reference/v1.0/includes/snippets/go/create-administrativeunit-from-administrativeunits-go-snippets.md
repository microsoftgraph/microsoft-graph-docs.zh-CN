---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c2fb87b1289ed2330623f8359b612283091ec91
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099179"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "Seattle District Technical Schools"
requestBody.SetDisplayName(&displayName)
description := "Seattle district technical schools administration"
requestBody.SetDescription(&description)
visibility := "HiddenMembership"
requestBody.SetVisibility(&visibility)
options := &msgraphsdk.AdministrativeUnitsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().AdministrativeUnits().Post(options)


```