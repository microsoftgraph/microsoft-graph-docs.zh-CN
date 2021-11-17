---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c66526a375ed47a254a36e7d8f25ac5864aec587
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978603"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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