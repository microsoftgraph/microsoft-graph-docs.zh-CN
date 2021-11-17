---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd5e52f7fb709853e347045b23fed2c102f6495a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991421"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
result, err := graphClient.AdministrativeUnits().Post(options)


```