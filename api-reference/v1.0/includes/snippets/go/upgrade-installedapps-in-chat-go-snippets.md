---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8277cf3b338f8adbfd25a85a787239073e14acf7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412462"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.ChatsById(&chatId).InstalledAppsById(&teamsAppInstallationId).Upgrade(chat-id, teamsAppInstallation-id).Post(nil)


```