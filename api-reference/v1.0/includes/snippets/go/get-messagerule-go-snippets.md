---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a511f1458cffa7aa960efc6d0dfb6bbffb2aaa7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288019"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Get(nil)


```