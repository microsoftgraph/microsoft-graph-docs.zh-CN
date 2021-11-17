---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d38a41d6e2f658a38484b2591db3b4e1f5a670a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978540"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.ChatsById(&chatId).InstalledAppsById(&teamsAppInstallationId).Delete(options)


```