---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cacb0999fd67d5f50411bb518b2114479335940e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327777"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Get()


```