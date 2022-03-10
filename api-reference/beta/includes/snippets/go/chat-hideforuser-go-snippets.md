---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 262f9baf23961b9c2cc586efbadac70705b816d9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411918"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
user := msgraphsdk.NewTeamworkUserIdentity()
requestBody.SetUser(user)
id := "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
user.SetId(&id)
tenantId := "2a690434-97d9-4eed-83a6-f5f13600199a"
requestBody.SetTenantId(&tenantId)
options := &msgraphsdk.HideForUserRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).HideForUser(chat-id).Post(options)


```