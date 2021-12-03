---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b18d66744e99b351917896018e54c425d17cf4f6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288519"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Delete(nil)


```