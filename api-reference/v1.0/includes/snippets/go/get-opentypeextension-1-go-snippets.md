---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdc5e871d9a555080117dfe9e79510bad2dfaa8e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095595"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
result, err := graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Get(options)


```