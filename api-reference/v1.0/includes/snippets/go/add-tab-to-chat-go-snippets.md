---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a38a10be779c8c9904a0aa264aa2d54fe0101560
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamsTab()
displayName := "My Contoso Tab"
requestBody.SetDisplayName(&displayName)
configuration := msgraphsdk.NewTeamsTabConfiguration()
requestBody.SetConfiguration(configuration)
entityId := "2DCA2E6C7A10415CAF6B8AB6661B3154"
configuration.SetEntityId(&entityId)
contentUrl := "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView"
configuration.SetContentUrl(&contentUrl)
websiteUrl := "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154"
configuration.SetWebsiteUrl(&websiteUrl)
removeUrl := "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
configuration.SetRemoveUrl(&removeUrl)
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
}
options := &msgraphsdk.TabsRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Tabs().Post(options)


```