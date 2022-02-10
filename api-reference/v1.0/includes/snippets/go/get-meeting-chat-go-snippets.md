---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cef783b1c4f1677a95e990738cdc1583c742d1c
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Get(nil)


```