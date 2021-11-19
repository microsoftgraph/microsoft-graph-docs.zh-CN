---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 159ea178efc9d0fbb41177d6bd578addf4f7dfff
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098134"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
currentPassword := "xWwvJ]6NMw+bWH-d"
requestBody.SetCurrentPassword(&currentPassword)
newPassword := "0eM85N54wFxWwvJ]"
requestBody.SetNewPassword(&newPassword)
options := &msgraphsdk.ChangePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().ChangePassword().Post(options)


```